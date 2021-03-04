---
title: 协议资源类型
description: 表示租户的可自定义使用条款协议，该协议是使用 Azure AD (Azure Active Directory) 。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: bb1de9d03de4d891ef91d076ccbd41e6b569e3f8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433199"
---
# <a name="agreement-resource-type"></a>协议资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户的可自定义使用条款协议，该协议是使用 Azure AD (Azure Active Directory) 。 可以使用以下方法根据你的方案创建和管理 Azure [Active Directory](/azure/active-directory/active-directory-tou) 使用条款功能。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建协议](../api/agreement-post-agreements.md) | [协议](agreement.md) | 通过发布到协议集合创建新协议。 |
| [列出协议](../api/agreement-list.md) | [协议](agreement.md) 集合 | 获取协议对象集合。 |
| [获取协议](../api/agreement-get.md) | [协议](agreement.md) | 读取协议对象的属性和关系。 |
| [更新协议](../api/agreement-update.md) | [协议](agreement.md) | 更新协议对象。 |
| [删除协议](../api/agreement-delete.md) | 无 | 删除协议对象。 |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|displayName|String|协议的显示名称。 此显示名称用于协议的内部跟踪，但不向查看协议的最终用户显示。|
|id|String| 只读。|
|isPerDeviceAcceptanceRequired|布尔|此设置使你能够要求最终用户在从其访问它的每个设备上接受此协议。 如果最终用户尚未在 Azure AD 中注册其设备，则要求他们这样做。|
|isViewingBeforeAcceptanceRequired|布尔|指示用户是否必须扩大协议才能接受。|
|termsExpiration|[termsExpiration](termsexpiration.md)| 所有用户的过期日程安排和协议频率。 |
|userReacceptRequiredFrequency|持续时间|用户必须重新接受使用条款的持续时间。 该值以 ISO 8601 格式表示，持续时间。|


## <a name="relationships"></a>关系
| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|接受|[agreementAcceptance](agreementacceptance.md) 集合|只读。 有关接受本协议的信息。|
|files|[agreementFileLocalization](agreementfilelocalization.md) 集合| 链接到本协议的 PDF。 **注意：** 此属性正在被弃用。 请  **改为使用文件** 属性。|
|file|[agreementFile](agreementfile.md) | 链接到本协议的默认 PDF。|
|文件/本地化|[agreementFileLocalization](agreementfilelocalization.md) 集合|附加到协议的协议文件的本地化版本。|
|file/localizations/{localizationId}/versions|[agreementFileVersion](agreementfileversion.md) 集合|本地化协议文件的版本历史记录。|


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


