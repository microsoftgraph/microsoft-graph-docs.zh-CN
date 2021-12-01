---
author: tushar20
title: sharePointIdentitySet 资源类型
ms.localizationpriority: medium
description: 表示 sharePointIdentity 和标识资源的键值集合。
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f8bf2e51c1b4af1935b5885ac91b767e444691e5
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242286"
---
# <a name="sharepointidentityset-resource-type"></a>sharePointIdentitySet 资源类型

表示 [sharePointIdentity 资源的键值](sharePointIdentity.md) 集合。 此资源从 **identitySet** 资源扩展，以提供向SharePoint特定信息的能力。

此资源用于表示与项目的各种事件关联的一组标识，例如由 创建或 _上次修改者_。 

有关使用情况信息，请参阅 [driveItem][]。

## <a name="properties"></a>属性

| 属性    | 类型                   | 说明 |
|:------------|:-----------------------|:----------------------------------------------------------- |
| application | [Identity][]           | 与此操作关联的应用程序。 可选。 |
| 设备      | [identity][]           | 与此操作关联的设备。 可选。 |
| 组       | [identity][]           | 与此操作关联的组。 可选。 |
| 用户        | [identity][]           | 与此操作关联的用户。 可选。 |
| siteUser    | [sharePointIdentity][] | 与SharePoint关联的用户。 可选。 |
| siteGroup   | [sharePointIdentity][] | 与SharePoint关联的组。 可选。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.sharePointIdentitySet",
       "optionalProperties": ["user", "application", "group", "device", "siteUser", "siteGroup"],
       "openType": true } -->

```json
{
  /** inherited from IdentitySet **/
  "application": {"@odata.type": "microsoft.graph.identity"},
  "device": {"@odata.type": "microsoft.graph.identity"},
  "user": {"@odata.type": "microsoft.graph.identity"},
  
  "group": {"@odata.type": "microsoft.graph.identity"},
  "siteUser": {"@odata.type": "microsoft.graph.sharePointIdentity"},
  "siteGroup":{"@odata.type": "microsoft.graph.sharePointIdentity"}
}
```

[driveItem]: driveItem.md
[identity]: identity.md
[sharePointIdentity]: sharePointIdentity.md

<!-- {
  "type": "#page.annotation",
  "description": "SharePointIdentity set is a collection of identities/sharePointIdentities",
  "section": "documentation",
  "tocPath&quot;: &quot;Resources/SharePointIdentitySet"
} -->
