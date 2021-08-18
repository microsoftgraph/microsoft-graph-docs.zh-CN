---
title: appleOwnerTypeEnrollmentType 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e0ee14009f1e43c3a7c06f9e9939cda0957009030115ce8c85faf975c20ad649
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54161183"
---
# <a name="appleownertypeenrollmenttype-resource-type"></a>appleOwnerTypeEnrollmentType 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ownerType|[managedDeviceOwnerType](../resources/intune-shared-manageddeviceownertype.md)|所有者类型。 可取值为：`unknown`、`company`、`personal`。|
|enrollmentType|[appleUserInitiatedEnrollmentType](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|注册类型。 可取值为：`unknown`、`device`、`user`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appleOwnerTypeEnrollmentType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleOwnerTypeEnrollmentType",
  "ownerType": "String",
  "enrollmentType": "String"
}
```




