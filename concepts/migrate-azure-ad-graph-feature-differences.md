---
title: Azure AD Graph 与 Microsoft Graph 之间的功能差异
description: 介绍了 Azure Active Directory （Azure AD） API 与 Microsoft Graph API 之间的功能差异，以帮助你快速轻松地迁移应用。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 531b2c9b441f328118597802b6478d5b45276965
ms.sourcegitcommit: 0545b031585e605dc3a0fde481015f51f79819c4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2020
ms.locfileid: "45224876"
---
# <a name="feature-differences-between-azure-ad-graph-and-microsoft-graph"></a>Azure AD Graph 与 Microsoft Graph 之间的功能差异

本文是*第1步：查看*[迁移应用程序](migrate-azure-ad-graph-planning-checklist.md)的 API 差异的过程的一部分。

Microsoft Graph 中的许多功能与 Azure AD Graph 对应的工作方式类似。 不过，已经更改和/或改进了少数几个部分。 在这里，你将了解如何改编你的应用以利用这些差异。  通常情况下，更改很小，但值得努力。

本文探讨 Microsoft Graph 如何处理以下内容：

- 目录架构扩展
- 差异查询
- 批处理

## <a name="directory-schema-extensions"></a>目录架构扩展

如果您的应用程序使用 Azure AD Graph 目录架构扩展，则可以继续使用相同的基本 Api （使用 Microsoft Graph 请求 Url）执行以下操作：

- 使用 [application] [/graph/api/resources/application？ view = graph-rest-extensionProperties 1.0）资源上的**extensionProperties**属性管理扩展属性定义。
- 使用[getAvailableExtensionProperties](/graph/api/directoryobject-getavailableextensionproperties?view=graph-rest-v1.0)操作获取可用扩展属性。
- 使用 GET 和，读取扩展值`$select`
- 使用 GET 和，搜索扩展值`$filter`
- 使用修补程序更新扩展值
- 使用修补程序删除扩展值（设置为**null**）

Microsoft Graph 提供了增强的架构扩展开发人员体验，这与 Azure AD Graph 目录架构 extentions 目前不是向后兼容。 若要了解详细信息，请参阅[添加自定义数据中的架构扩展](/graph/extensibility-overview#schema-extensions)。

### <a name="recommended-migration-approach"></a>建议的迁移方法

如果你的 Azure AD Graph 应用使用目录架构扩展，请采用增量方法将应用迁移到 Microsoft Graph。

首先，将您的应用程序切换为使用 Microsoft Graph API 调用，但让应用继续利用 Azure AD Graph 目录架构扩展。

然后，您可以切换到使用 Microsoft Graph 架构扩展。 在某些情况下，切换将不合适。 请勿切换（如果有）：

- 您的应用程序使用通过 AD Connect 创建的目录架构扩展，或者
- 您的应用程序依赖于令牌声明中的目录架构扩展值。

>**注意**：尚不支持使用 Microsoft Graph 架构扩展属性作为令牌中使用可选声明或动态成员身份规则的声明。

若要切换到较新的 Microsoft Graph 架构扩展模型，需要执行以下操作：

- 使用 Microsoft Graph 定义新的架构扩展定义。
- 更新应用程序以支持新的架构扩展定义。
- 将数据从 Azure AD 架构扩展属性迁移到新的 Microsoft Graph 架构扩展属性。  不支持自动迁移数据。

## <a name="differential-queries"></a>差异查询

Azure AD Graph 和 Microsoft Graph 让你可以使用查询跟踪更改。  这两个 Api 的高级别方法类似，但语法不同。

Azure AD Graph 调用这些差异查询。  在 Microsoft Graph 中，它们是[delta 查询](/graph/delta-query-overview)。

下表重点介绍了主要的相似之处和差异：

|Delta 请求 |Azure AD Graph | Microsoft Graph |
|----|----|----|
| _初始数据请求_ | 使用查询参数：<br>`GET /groups?deltaLink=` | 使用函数： <br> `GET /groups/delta` |
| _获取新更改_ | `GET /groups?deltaLink={deltaToken}` | `GET /groups/delta?$deltaToken={deltaToken}` |
| _从现在开始同步_ |使用自定义 HTTP 标头：<br> `ocp-aad-dq-include-only-delta-token: true` | 使用查询参数： <br> `GET /groups/delta?$deltaToken=latest` |
| _跟踪 directoryObjects 的更改_ | 获取相同操作中的多个资源（用户和组）的更改：&nbsp;&nbsp;<br> `GET /directoryObject?$filter=isof('User') or isof('Group')&deltaLink=` | 将单独的查询与 Microsoft Graph 结合使用，每个资源对应一项。 |
| _获取资源和关系更改_ | 如果资源有关系，所有请求都将返回资源和关系更改。 | `GET /groups/delta?$expand=members` |
| _指示新项目和已更改项目的响应_ | <ul><li><p>使用其标准表示形式表示新创建的实例。</p></li><li><p>更新后的实例由其 id 表示，*至少*具有已更新的属性。 可以包含其他属性。</p></li><li><p>关系表示为 `directoryLinkChange` 类型。</p></li></ul>|<ul><li><p>使用其标准表示形式表示新创建的实例。</p></li><li><p>更新后的实例由其 id 表示，*至少*具有已更新的属性。 可以包含其他属性。</p></li><li><p>关系表示为标准资源表示形式的批注。 这些批注使用格式 `propertyName@delta` ，例如， `members@delta` 组的成员资格更改。</p></li></ul> |
| _指示已删除项目的响应_| 指示一个已删除的项，其附加属性为*isDeleted*设置为 true。 | 指示已删除的项目和 \@ 已删除的注释。 它还可能包含原因代码，以指示是否已删除项目，但可以还原或永久删除。 |

如果您的应用程序已在存储状态数据，请考虑使用前面所示的 "从现在同步"，以帮助管理到增量查询的转换。

## <a name="batching"></a>批处理

Azure AD Graph 使用称为多部分 MIME 邮件的系统来管理批处理。  Microsoft Graph 使用[JSON 批处理](json-batching.md)在单个批处理操作中允许最长20个请求。 JSON 批处理机制使用起来明显简单，尤其是 JSON 分析库。  它还允许对批处理操作进行排序。  但是，与 Azure AD Graph 批处理方法相比，它不是向后兼容。

## <a name="next-steps"></a>后续步骤

- 了解 Azure AD Graph 与 Microsoft Graph 之间的[资源差异](migrate-azure-ad-graph-resource-differences.md)。
- 探索[添加自定义数据](/graph/extensibility-overview)，以获取有关开放和架构扩展的信息。
- 浏览[delta 查询](/graph/delta-query-overview)以了解 Microsoft Graph 的差异查询版本。
- 浏览[JSON 批处理](json-batching.md)以了解批处理在 Microsoft Graph 中的工作方式。
- 使用[Graph 浏览器](https://aka.ms/ge)试用 Microsoft Graph。

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: /concepts/migrate-azure-ad-graph-feature-changes.md:
      Failed to parse any rows out of table with headers: |Task|Azure AD Graph|Microsoft Graph|"
  ],
}
-->
