# [hackettyu'note] Code pusudown 准则

利用SELECT COUNT直接在数据库层完成统计工作。这也是SAP推荐的做法，所谓Code pusudown准则，即能放到HANA数据库层面进行的操作，就尽量放进去，以充分利用HANA强大的计算能力。在数据库能够完成计算逻辑的前提下，尽量避免把计算逻辑放到Netweaver ABAP应用层去做。