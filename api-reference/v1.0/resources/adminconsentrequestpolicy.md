---
title: adminConsentRequestPolicy 资源类型
description: 指定可在整个租户中创建和管理同意请求的策略。
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d2c4bffc0de82f4bdb55186db76dc0eb0fe17ff77e3edf6cc1b0d6fddcf32d68
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54202551"
---
# <a name="adminconsentrequestpolicy-resource-type"></a>adminConsentRequestPolicy 资源类型

命名空间：microsoft.graph

指定创建和管理整个租户的同意请求的策略。 每个租户只有一个 **adminConsentRequestPolicy。**

**adminConsentRequestPolicy** 在创建同意请求时提供其他设置，以控制启动同意请求时的功能行为。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[获取 adminConsentRequestPolicy](../api/adminconsentrequestpolicy-get.md)|[adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md)|读取 [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) 对象的属性和关系。|
|[更新 adminConsentRequestPolicy](../api/adminconsentrequestpolicy-update.md)|[adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md)|更新 [adminConsentRequestPolicy 对象](../resources/adminconsentrequestpolicy.md) 的属性。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|isEnabled|Boolean|指定是启用还是禁用管理员同意请求功能。 必填。|
|notifyReviewers|Boolean|指定审阅者是否将收到通知。 必填。|
|remindersEnabled|Boolean|指定审阅者是否将收到提醒电子邮件。 必填。|
|requestDurationInDays|Int32|指定请求在未应用决策时自动过期之前处于活动状态的持续时间。|
|reviewers|[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合|管理员同意的审阅者列表。 必填。|
|version|Int32|指定此策略的版本。 更新策略时，将更新此版本。 只读。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.adminConsentRequestPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsentRequestPolicy",
  "isEnabled": "Boolean",
  "version": "Integer",
  "notifyReviewers": "Boolean",
  "remindersEnabled": "Boolean",
  "requestDurationInDays": "Integer",
  "reviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ]
}
```

