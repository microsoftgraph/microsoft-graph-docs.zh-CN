---
title: 协议资源类型
description: 表示使用 Azure AD (Azure Active Directory 创建和管理的租户可自定义) 。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 045d4b9142d4bd0c4bc01392975871e0253d33c0
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722620"
---
# <a name="agreement-resource-type"></a>协议资源类型

命名空间：microsoft.graph

表示使用 Azure AD (Azure Active Directory 创建和管理的租户可自定义) 。 可以使用以下方法根据你的方案创建和管理 Azure [Active Directory](/azure/active-directory/active-directory-tou) 使用条款功能。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出协议](../api/agreement-list.md) | [协议](agreement.md) 集合 | 获取协议对象集合。 |
| [创建协议](../api/agreement-post-agreements.md) | [协议](agreement.md) | 通过发布到协议集合创建新协议。 |
| [获取协议](../api/agreement-get.md) | [协议](agreement.md) | 读取协议对象的属性和关系。 |
| [更新协议](../api/agreement-update.md) | [协议](agreement.md) | 更新协议对象。 |
| [删除协议](../api/agreement-delete.md) | 无 | 删除协议对象。 |

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|displayName|字符串|协议的显示名称。 The 显示名称 is used for internal tracking of the agreement but is not shown to end users who view the agreement.|
|id|字符串| 协议的标识符。 只读。|
|isPerDeviceAcceptanceRequired|布尔值|指示最终用户是否需要在从其访问它的每个设备上接受此协议。 如果最终用户尚未在 Azure AD 中注册其设备，则要求他们这样做。|
|isViewingBeforeAcceptanceRequired|布尔值|指示用户是否必须扩展协议才能接受。|
|termsExpiration|[termsExpiration](termsexpiration.md)| 所有用户的过期日程安排和协议频率。 |
|userReacceptRequiredFrequency|持续时间|用户必须重新接受使用条款的持续时间。 该值以 ISO 8601 格式表示持续时间。|


## <a name="relationships"></a>关系
| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|接受|[agreementAcceptance](agreementacceptance.md) 集合|只读。 有关接受本协议的信息。|
|files|[agreementFileLocalization](agreementfilelocalization.md) 集合| 链接到本协议的 PDF。 此属性正在被弃用。 请  **改为使用 file** 属性。|
|file|[agreementFile](agreementfile.md) | 链接到本协议的默认 PDF。|
|本地化|[agreementFileLocalization](agreementfilelocalization.md) 集合|附加到该协议的协议文件的本地化版本。|
|版本|[agreementFileVersion](agreementfileversion.md) 集合|本地化协议文件的版本历史记录。|


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


