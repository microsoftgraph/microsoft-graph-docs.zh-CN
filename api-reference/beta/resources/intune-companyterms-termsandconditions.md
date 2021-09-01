---
title: termsAndConditions 资源类型
description: TermsAndConditions 实体表示给定条款和条件 (T&C) 策略的元数据和内容。 当用户第一次尝试注册到 Intune 时向用户显示 T&C 策略的内容，之后会在进行了管理员要求重新接受的编辑时显示。 这允许管理员与用户必须同意的预配进行通信，以便将设备注册到 Intune 中。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 723476aa9edaea09ca0bbc916fe63a57a64c3460
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58820518"
---
# <a name="termsandconditions-resource-type"></a>termsAndConditions 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

TermsAndConditions 实体表示给定条款和条件 (T&C) 策略的元数据和内容。 当用户第一次尝试注册到 Intune 时向用户显示 T&C 策略的内容，之后会在进行了管理员要求重新接受的编辑时显示。 这允许管理员与用户必须同意的预配进行通信，以便将设备注册到 Intune 中。

## <a name="methods"></a>方法
|方法|返回类型|Description|
|:---|:---|:---|
|[List termsAndConditionses](../api/intune-companyterms-termsandconditions-list.md)|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 集合|列出 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性和关系。|
|[Get termsAndConditions](../api/intune-companyterms-termsandconditions-get.md)|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|读取 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性和关系。|
|[Create termsAndConditions](../api/intune-companyterms-termsandconditions-create.md)|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|创建新的 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象。|
|[Delete termsAndConditions](../api/intune-companyterms-termsandconditions-delete.md)|无|删除 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)。|
|[Update termsAndConditions](../api/intune-companyterms-termsandconditions-update.md)|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|更新 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|T&C 策略的唯一标识符。|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。|
|modifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。|
|displayName|String|管理员提供的 T&C 策略名称。 |
|description|字符串|管理员提供的 T&C 策略描述。|
|title|String|管理员提供的条款和条件标题。 这会向用户显示，提示用户接受 T&C 策略。|
|bodyText|String|管理员提供的条款和条件正文文本，通常为条款本身。 这会向用户显示，提示用户接受 T&C 策略。|
|acceptanceStatement|String|管理员提供的条款和条件说明，通常会说明接受 T&C 策略中陈述的条款和条件意味着什么。 这会向用户显示，提示用户接受 T&C 策略。|
|version|Int32|指示当前条款版本的整数。 当管理员对条款进行更改，并希望要求用户重新接受修改的 T&C 策略时会递增。|
|roleScopeTagIds|字符串集合|此实体实例的范围标记列表。|

## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|groupAssignments|[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) 集合|此 T 策略的组分配&C 策略。|
|assignments|[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 集合|此 T&C 策略的分配列表。|
|acceptanceStatuses|[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 集合|此 T&C 策略的接受状态列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "title": "String",
  "bodyText": "String",
  "acceptanceStatement": "String",
  "version": 1024,
  "roleScopeTagIds": [
    "String"
  ]
}
```



