---
title: Azure AD Graph 和 Microsoft Graph 之间的功能差异
description: 介绍 Azure Active Directory (Azure AD) 图形 API与 Microsoft 图形 API 之间的功能差异，以帮助你快速轻松地迁移应用。
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: 4ed6de06843d33c80dfcab28c885b7242ceede29
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2022
ms.locfileid: "66555742"
---
# <a name="feature-differences-between-azure-ad-graph-and-microsoft-graph"></a>Azure AD Graph 和 Microsoft Graph 之间的功能差异

本文是 *步骤 1 的一部分：查看*[迁移应用的过程](migrate-azure-ad-graph-planning-checklist.md)的 API 差异。

Microsoft Graph 中的许多功能的工作方式与 Azure AD (Azure AD) Graph 对应的 Azure Active Directory 类似。 但是，一些已更改或改进。 在这里，你将了解如何调整应用以利用这些差异。  通常，更改是次要的，但非常值得努力。

本文探讨 Microsoft Graph 如何处理：

- 目录架构扩展
- 差异查询
- 批处理

## <a name="directory-extensions"></a>目录扩展

如果应用使用 Azure AD Graph 目录扩展，则可以继续使用与 Microsoft Graph 请求 URL 相同的基本 API () ：

- 使用 [extensionProperty](/graph/api/resources/extensionproperty) 资源和关联的方法管理目录扩展定义。
- 使用 [getAvailableExtensionProperties](/graph/api/directoryobject-getavailableextensionproperties) 操作获取可用扩展属性。
- 使用 GET 和用户读取扩展值，仅 `$select` 通过 `v1.0` 终结点通过查询读取扩展值
- 使用 GET 搜索扩展值和 `$filter`
- 使用 PATCH 更新扩展值
- 使用 PATCH (设置为 **null**) 删除扩展值

Microsoft Graph 提供增强的架构扩展开发人员体验，目前与 Azure AD Graph 目录扩展不向后兼容。 若要了解详细信息，请参阅 [为应用程序选择扩展类型](extensibility-overview.md#choose-an-extension-type-for-your-application)。

### <a name="recommended-migration-approach"></a>建议的迁移方法

如果 Azure AD Graph 应用使用目录扩展，请采用增量方法将应用迁移到 Microsoft Graph。

首先，将应用切换到使用 Microsoft 图形 API调用，但让应用继续利用 Azure AD Graph 目录扩展。

然后，可以切换到使用 Microsoft Graph 架构扩展。 在某些情况下，切换将不合适。 如果：

- 应用使用通过 AD Connect 创建的目录扩展
- 应用设置其他应用在令牌声明中使用的目录扩展值
- 应用设置动态成员身份规则中使用的目录扩展值 

>**注意**：尚不支持使用可选声明或动态成员身份规则将 Microsoft Graph 架构扩展属性用作令牌中的声明。

若要切换到较新的 Microsoft Graph 架构扩展模型，需要：

- 使用 Microsoft Graph 定义新的架构扩展定义。
- 更新应用以支持新的架构扩展定义。
- 将数据从 Azure AD 架构扩展属性迁移到新的 Microsoft Graph 架构扩展属性。  不支持自动迁移数据。

## <a name="differential-queries"></a>差异查询

使用 Azure AD Graph 和 Microsoft Graph 可以使用查询跟踪更改。  这两个 API 之间的高级方法类似，但语法不同。

Azure AD Graph 调用这些差异查询。  在 Microsoft Graph 中，它们是 [增量查询](./delta-query-overview.md)。

下表突出显示了关键相似之处和差异：

|增量请求 |Azure AD Graph | Microsoft Graph |
|----|----|----|
| _初始数据请求_ | 使用查询参数：<br>`GET /groups?deltaLink=` | 使用函数： <br> `GET /groups/delta` |
| _获取新更改_ | `GET /groups?deltaLink={deltaToken}` | `GET /groups/delta?$deltaToken={deltaToken}` |
| _从现在起同步_ |使用自定义 HTTP 标头：<br> `ocp-aad-dq-include-only-delta-token: true` | 使用查询参数： <br> `GET /groups/delta?$deltaToken=latest` |
| _跟踪 directoryObjects 的更改_ | 获取同一操作中多个资源 (用户和组) 的更改：&nbsp;&nbsp;<br> `GET /directoryObject?$filter=isof('User') or isof('Group')&deltaLink=` | 对 Microsoft Graph 使用单独的查询，每个资源使用一个查询。 |
| _获取资源和关系更改_ | 如果资源具有关系，则所有请求都将返回资源和关系更改。 | `GET /groups/delta?$expand=members` |
| _指示新项和已更改项的响应_ | <ul><li><p>表示使用其标准表示形式新建的实例。</p></li><li><p>更新的实例的 ID *至少包含已* 更新的属性。 可能包含其他属性。</p></li><li><p>关系表示为 `directoryLinkChange` 类型。</p></li></ul>|<ul><li><p>表示使用其标准表示形式新建的实例。</p></li><li><p>更新的实例的 ID *至少包含已* 更新的属性。 可能包含其他属性。</p></li><li><p>关系表示为标准资源表示形式的注释。 这些批注使用格式 `propertyName@delta`，例如 `members@delta` 组的成员身份更改。</p></li></ul> |
| _指示已删除项的响应_| 指示已删除的项，其中 *aad.isDeleted* 的附加属性设置为 true。 | 指示包含已删除批注的 \@已删除项。 它还可能包含一个原因代码，该代码指示项目是否已删除，但可以还原或永久删除。 |

如果应用已存储状态数据，请考虑使用前面显示的“从现在开始同步”来帮助管理到增量查询的转换。

## <a name="batching"></a>批处理

Azure AD Graph 使用名为多部分 MIME 消息的系统来管理批处理。  Microsoft Graph 使用 [JSON 批处理](json-batching.md) 在单个批处理操作中最多允许 20 个请求。 JSON 批处理机制非常简单，尤其是与 JSON 分析库一起使用。  它还允许对批处理操作进行排序。  但是，它与 Azure AD Graph 批处理方法不向后兼容。

## <a name="next-steps"></a>后续步骤

- 了解 Azure AD Graph 和 Microsoft Graph 之间的 [资源差异](migrate-azure-ad-graph-resource-differences.md) 。
- 再次查看 [清单](migrate-azure-ad-graph-planning-checklist.md) 。

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: /concepts/migrate-azure-ad-graph-feature-changes.md:
      Failed to parse any rows out of table with headers: |Task|Azure AD Graph|Microsoft Graph|"
  ],
}
-->