# Shinya Aoi
# CSS 340 HW4
# 11/02/2018


def findTreasure(x1, y1, x2, y2):
    return helpFindTreasure(x1, y1, x2, y2, "", 0)


# This function is to find the path to the treasure recursively.
# This also finds the number of path to get to the treasure.
def helpFindTreasure(robX, robY, treX, treY, path, currentNumOfPath):
    if robX == treX and robY == treY:
        print(path)
        return currentNumOfPath + 1

    if robY < treY:
        currentNumOfPath = helpFindTreasure(robX, robY+1, treX, treY, path + "N", currentNumOfPath)

    if robY > treY:
        currentNumOfPath = helpFindTreasure(robX, robY-1, treX, treY, path + "S", currentNumOfPath)

    if robX < treX:
        currentNumOfPath = helpFindTreasure(robX+1, robY, treX, treY, path + "E", currentNumOfPath)

    if robX > treX:
        currentNumOfPath = helpFindTreasure(robX-1, robY, treX, treY, path + "W", currentNumOfPath)

    return currentNumOfPath
