---
title: 协议资源类型
description: 表示租户的可自定义使用条款协议，该协议是使用 Azure Active Directory (Azure AD) 。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 28abdafb3adda1b1fd3356fcdd1db5bda86c804f
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651377"
---
# <a name="agreement-resource-type"></a>协议资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户的可自定义使用条款协议，该协议是使用 Azure Active Directory (Azure AD) 。 您可以使用以下方法根据你的方案创建和管理Azure Active Directory[使用条款](/azure/active-directory/conditional-access/terms-of-use)"功能。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建协议](../api/termsofusecontainer-post-agreements.md) | [协议](agreement.md) | 通过发布到协议集合创建新协议。 |
| [列出协议](../api/termsofusecontainer-list-agreements.md) | [协议](agreement.md) 集合 | 获取协议对象集合。 |
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
|displayName|String|协议的显示名称。 The 显示名称 is used for internal tracking of the agreement but is not shown to end users who view the agreement.|
|id|String| 只读。|
|isPerDeviceAcceptanceRequired|Boolean|此设置使你能够要求最终用户在从其访问它的每个设备上接受此协议。 最终用户需要将设备注册到 Azure AD（如果他们尚未这样做）。|
|isViewingBeforeAcceptanceRequired|Boolean|指示用户是否必须扩展协议才能接受。|
|termsExpiration|[termsExpiration](termsexpiration.md)| 所有用户的过期日程安排和协议频率。 |
|userReacceptRequiredFrequency|期限|用户必须重新接受使用条款的持续时间。 该值以 ISO 8601 格式表示，持续时间为。|


## <a name="relationships"></a>关系
| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|接受|[agreementAcceptance](agreementacceptance.md) 集合|只读。 有关接受本协议的信息。|
|file|[agreementFile](agreementfile.md) | 链接到本协议的默认 PDF。|
|files|[agreementFileLocalization](agreementfilelocalization.md) 集合| 链接到本协议的 PDF。 **注意：** 此属性正在被弃用。 请  **改为使用 file** 属性。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.agreement",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.agreement",
  "id": "String (identifier)",
  "displayName": "String",
  "termsExpiration": {
    "@odata.type": "microsoft.graph.termsExpiration"
  },
  "userReacceptRequiredFrequency": "String (duration)",
  "isViewingBeforeAcceptanceRequired": "Boolean",
  "isPerDeviceAcceptanceRequired": "Boolean"
}
```
