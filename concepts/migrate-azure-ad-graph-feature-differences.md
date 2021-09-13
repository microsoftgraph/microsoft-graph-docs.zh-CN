---
title: Azure AD Azure Active Directory (和 Microsoft) Graph 之间的功能Graph
description: 介绍 Azure AD Azure Active Directory (API) Graph Microsoft Graph API 之间的功能差异，以帮助你快速轻松地迁移应用。
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: a615429eb3887970b00df211f592ec01f2009f23
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139147"
---
# <a name="feature-differences-between-azure-active-directory-azure-ad-graph-and-microsoft-graph"></a>Azure AD Azure Active Directory (和 Microsoft) Graph 之间的功能Graph

本文是步骤 *1：查看迁移应用的* 过程的 API [差异的一部分](migrate-azure-ad-graph-planning-checklist.md)。

Microsoft 中的许多功能Graph Azure AD 和对应项Graph类似。 但是，有一些已经过更改或改进。 在这里，你将了解如何调整应用以充分利用这些差异。  更改通常很小，但值得付出努力。

本文探讨 Microsoft Graph如何处理：

- 目录架构扩展
- 差异查询
- 批处理

## <a name="directory-schema-extensions"></a>目录架构扩展

如果你的应用使用 Azure AD Graph目录扩展，你可以继续使用与 Microsoft (请求 URL Graph相同的基本 API) ：

- 使用 [application][/graph/api/resources/application？view=graph-rest-v1.0 资源上的 **extensionProperties** 属性管理扩展) 定义。
- 使用 [getAvailableExtensionProperties](/graph/api/directoryobject-getavailableextensionproperties) 操作获取可用的扩展属性。
- 使用 GET 和 读取扩展值 `$select`
- 使用 GET 和 搜索扩展值 `$filter`
- 使用 PATCH 更新扩展值
- 使用 PATCH 删除扩展 (设置为 null **)**

Microsoft Graph 提供了增强的架构扩展开发人员体验，现在它无法向后兼容 Azure AD Graph目录扩展。 若要了解更多信息，请参阅 [添加自定义数据 中的架构扩展](./extensibility-overview.md#schema-extensions)。

### <a name="recommended-migration-approach"></a>建议的迁移方法

如果你的 Azure AD Graph应用使用目录扩展，请采用增量方法将应用迁移到 Microsoft Graph。

首先，将应用切换到使用 Microsoft Graph API 调用，但允许应用继续利用 Azure AD Graph目录扩展。

然后，你可以切换到使用 Microsoft Graph架构扩展。 在某些情况下，切换将不适合。 如果：

- 你的应用使用通过 AD 应用程序创建的目录连接
- 你的应用设置其他应用在令牌声明中使用的目录扩展值
- 你的应用设置动态成员资格规则中使用的目录扩展值 

>**注意**：Graph使用可选声明或动态成员资格规则将 Microsoft 架构扩展属性用作令牌中的声明。

若要切换到较新的 Microsoft Graph架构扩展模型，你需要：

- 使用 Microsoft 服务定义新的架构扩展Graph。
- 更新应用以支持新的架构扩展定义。
- 将数据从 Azure AD 架构扩展属性迁移到新的 Microsoft Graph架构扩展属性。  不支持自动迁移数据。

## <a name="differential-queries"></a>差异查询

Azure AD Graph 和 Microsoft Graph让你可以使用查询跟踪更改。  高级方法在两个 API 之间相似，但语法不同。

Azure AD Graph调用这些差异查询。  在 Microsoft Graph 中，它们是[delta 查询](./delta-query-overview.md)。

下表重点介绍了主要相似之处和区别：

|Delta 请求 |Azure AD Graph | Microsoft Graph |
|----|----|----|
| _初始数据请求_ | 使用查询参数：<br>`GET /groups?deltaLink=` | 使用 函数： <br> `GET /groups/delta` |
| _获取新更改_ | `GET /groups?deltaLink={deltaToken}` | `GET /groups/delta?$deltaToken={deltaToken}` |
| _从现在开始同步_ |使用自定义 HTTP 标头：<br> `ocp-aad-dq-include-only-delta-token: true` | 使用查询参数： <br> `GET /groups/delta?$deltaToken=latest` |
| _跟踪 directoryObjects 的更改_ | 在同一操作中 (多个资源组) 组更改：&nbsp;&nbsp;<br> `GET /directoryObject?$filter=isof('User') or isof('Group')&deltaLink=` | 将单独的查询与 Microsoft Graph，每个资源一个。 |
| _获取资源和关系更改_ | 如果资源具有关系，则所有请求都返回资源和关系更改。 | `GET /groups/delta?$expand=members` |
| _指示新项和已更改项的响应_ | <ul><li><p>表示使用其标准表示形式新建的实例。</p></li><li><p>更新的实例用其 ID 表示，其中 *至少* 具有已更新的属性。 也可以包括其他属性。</p></li><li><p>关系表示为 `directoryLinkChange` 类型。</p></li></ul>|<ul><li><p>表示使用其标准表示形式新建的实例。</p></li><li><p>更新的实例用其 ID 表示，其中 *至少* 具有已更新的属性。 也可以包括其他属性。</p></li><li><p>关系表示为对标准资源表示法的注释。 这些批注使用 格式 `propertyName@delta` ，例如 `members@delta` ，用于更改组的成员身份。</p></li></ul> |
| _指示已删除项目的响应_| 指示已删除的项目，其中 *aad.isDeleted* 的其他属性设置为 true。 | 指示具有已删除批注的 \@ 已删除项目。 它还可能包含原因代码，该代码指示项目是否被删除，但可以还原或永久删除。 |

如果你的应用已经存储状态数据，请考虑使用前面显示的"立即同步"来帮助管理到增量查询的过渡。

## <a name="batching"></a>批处理

Azure AD Graph使用名为多部分 MIME 邮件的系统来管理批处理。  Microsoft Graph 使用[JSON 批处理](json-batching.md)允许单个批处理操作中最多 20 个请求。 JSON 批处理机制使用起来要简单许多，尤其是与 JSON 分析库一起使用。  它还允许排序批处理操作。  但是，它不能向后兼容 Azure AD Graph批处理方法。

## <a name="next-steps"></a>后续步骤

- 了解 Azure AD[应用程序](migrate-azure-ad-graph-resource-differences.md)与 Microsoft Graph 之间的资源Graph。
- 再次查看 [检查](migrate-azure-ad-graph-planning-checklist.md) 表。

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: /concepts/migrate-azure-ad-graph-feature-changes.md:
      Failed to parse any rows out of table with headers: |Task|Azure AD Graph|Microsoft Graph|"
  ],
}
-->