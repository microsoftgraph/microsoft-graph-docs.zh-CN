---
title: userSettings 资源类型
description: '内容发现的当前用户设置。 '
author: jpettere
ms.localizationpriority: high
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: d003e700947b21014328268264e182c8bc1b97b1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139546"
---
# <a name="usersettings-resource-type"></a>userSettings 资源类型

命名空间：microsoft.graph

内容发现的当前用户设置。
若要了解如何获取或更新用户设置，请参阅[获取设置](../api/usersettings-get.md)和[更新设置](../api/usersettings-update.md)。

该资源支持：

- 检查用户及用户的组织是否对内容发现做贡献。
- 为特定用户禁用或启用内容发现。 这也会禁用 Office Delve 中的文档。

> [!NOTE]
> 此终结点仅适用于用户。 无法将此终结点用于联系人。

## <a name="methods"></a>方法
| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取用户设置](../api/usersettings-get.md) |[userSettings](../resources/usersettings.md)| 获取用户和组织设置。 |
|[更新用户设置](../api/usersettings-update.md) |[userSettings](../resources/usersettings.md)| 更新用户当前的设置。 |

## <a name="properties"></a>属性

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|contributionToContentDiscoveryDisabled|布尔值|如果设为 true，则会禁用至用户的[趋势](/graph/api/resources/insights-trending?view=graph-rest-beta) API 的委托访问。 如果设为 true，则用户的 Office Delve 中的文档将禁用。 如果设为 true，则 Microsoft 365 中显示的内容相关性（如 SharePoint 家庭版中的建议网站以及 OneDrive for Business 中的发现视图）将受到影响。 用户可以在 [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout) 中控制此设置。 |
|contributionToContentDiscoveryAsOrganizationDisabled|布尔值|反映用于控制至[趋势](/graph/api/resources/insights-trending?view=graph-rest-beta) API 的委托访问的[组织级别设置](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff)。 如果设为 true，则组织没有 Office Delve 的访问权限。 对整个组织来说，Microsoft 365 中显示的内容相关性（如 SharePoint 家庭版中的建议网站以及 OneDrive for Business 中的发现视图）将受到影响。 此设置为只读，并且仅可由管理员在 [SharePoint 管理中心](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US)更改。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```

