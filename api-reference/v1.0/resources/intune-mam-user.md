---
title: 用户资源类型
description: 表示 Azure Active Directory 用户对象。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f8aa697e8094c9468c92fd11a3c19dc4cf77bcc2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118066"
---
# <a name="user-resource-type"></a>用户资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 Azure Active Directory 用户对象。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List users](../api/intune-mam-user-list.md)|[user](../resources/intune-mam-user.md) 集合|列出 [user](../resources/intune-mam-user.md) 对象的属性和关系。|
|[Get user](../api/intune-mam-user-get.md)|[user](../resources/intune-mam-user.md)|读取 [user](../resources/intune-mam-user.md) 对象的属性和关系。|
|[Create user](../api/intune-mam-user-create.md)|[user](../resources/intune-mam-user.md)|创建新的 [user](../resources/intune-mam-user.md) 对象。|
|[Delete user](../api/intune-mam-user-delete.md)|None|删除 [user](../resources/intune-mam-user.md)。|
|[Update user](../api/intune-mam-user-update.md)|[user](../resources/intune-mam-user.md)|更新 [user](../resources/intune-mam-user.md) 对象的属性。|
|[getManagedAppDiagnosticStatuses 函数](../api/intune-mam-user-getmanagedappdiagnosticstatuses.md)|[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) 集合|获取给定用户的诊断验证状态。|
|[getManagedAppPolicies 函数](../api/intune-mam-user-getmanagedapppolicies.md)|[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合|获取给定用户的应用限制。|
|[wipeManagedAppRegistrationsByDeviceTag 操作](../api/intune-mam-user-wipemanagedappregistrationsbydevicetag.md)|无|对含有指定设备标记的应用注册发布擦除操作。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户标识符。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|managedAppRegistrations|[managedAppRegistration](../resources/intune-mam-managedappregistration.md) 集合|属于用户的零个或多个托管的应用注册。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```




