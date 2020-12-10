---
title: 协议资源类型
description: 表示租户的可自定义使用条款协议，该协议是使用 Azure Active Directory (Azure AD) 创建和管理的。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: af4a6079aaed846af3322a94eb961315f7291686
ms.sourcegitcommit: d9c167f6be71bdb4a023c5ace2733b9854c846d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617099"
---
# <a name="agreement-resource-type"></a>协议资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户的可自定义使用条款协议，该协议是使用 Azure Active Directory (Azure AD) 创建和管理的。 您可以根据您的方案使用以下方法来创建和管理 [Azure Active Directory 使用条款功能](/azure/active-directory/active-directory-tou) 。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建协议](../api/agreement-post-agreements.md) | [本](agreement.md) | 通过发布到协议集合创建新协议。 |
| [列出协议](../api/agreement-list.md) | [协议](agreement.md) 集合 | 获取一个协议对象集合。 |
| [获取协议](../api/agreement-get.md) | [本](agreement.md) | 读取协议对象的属性和关系。 |
| [更新协议](../api/agreement-update.md) | [本](agreement.md) | 更新协议对象。 |
| [删除协议](../api/agreement-delete.md) | 无 | 删除协议对象。 |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|displayName|String|协议的显示名称。 显示名称用于协议的内部跟踪，但不向查看该协议的最终用户显示。|
|id|String| 只读。|
|isPerDeviceAcceptanceRequired|布尔值|通过此设置，您可以要求最终用户在其访问它的每台设备上接受此协议。 最终用户将需要在 Azure AD 中注册其设备（如果尚未这样做）。|
|isViewingBeforeAcceptanceRequired|布尔值|指示用户是否必须在接受前展开协议。|
|termsExpiration|[termsExpiration](termsexpiration.md)| 所有用户的到期计划和协议频率。 |
|userReacceptRequiredFrequency|持续时间|持续时间，用户必须重新接受使用条款。 值以 ISO 8601 格式表示，持续时间。|


## <a name="relationships"></a>关系
| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|acceptances|[agreementAcceptance](agreementacceptance.md) 集合|只读。 本协议 acceptances 的相关信息。|
|files|[agreementFileLocalization](agreementfilelocalization.md) 集合| 链接到此协议的 Pdf。 **注意：** 此属性正处于弃用的过程中。 请改为使用  **file** 属性。|
|file|[agreementFile](agreementfile.md) | 链接到此协议的默认 PDF。|
|file/localizations|[agreementFileLocalization](agreementfilelocalization.md) 集合|附加到协议的协议文件的本地化版本。|
|file/localizations/{localizationId}/版本|[agreementFileVersion](agreementfileversion.md) 集合|本地化协议文件的版本历史记录。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreement"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "isPerDeviceAcceptanceRequired": false,
  "termsExpiration": {
    "startDateTime": "2018-10-01T00:00:00.0000000Z",
    "frequency": "PT1M"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


