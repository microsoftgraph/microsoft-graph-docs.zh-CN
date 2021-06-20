
<!-- markdownlint-disable MD041-->

当应用程序查询返回 directoryObject 类型集合的关系时，如果它没有读取某种派生类型（如设备）的权限，则会返回该类型的成员，但返回的信息有限。 使用这种行为，应用程序可请求所需的最低特权权限，而不依赖于 *Directory.** 集权限。 有关详细信息，请参阅[为不可访问的成员对象返回有限的信息](/graph/permissions-reference#limited-information-returned-for-inaccessible-member-objects)。

