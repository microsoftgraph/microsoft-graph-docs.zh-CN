
<!-- markdownlint-disable MD041-->

当应用程序查询一个返回 directoryObject 类型集合的关系时，如果它没有读取某个派生类型（如设备）的权限，则返回该类型的成员，但不包含有限的信息。 使用此行为，应用程序可以请求所需的最少特权权限，而不是依赖于目录集。 * 权限。 有关详细信息，请参阅[为不可访问的成员对象返回的受限制的信息](/graph/permissions-reference#limited-information-returned-for-inaccessible-member-objects)。

