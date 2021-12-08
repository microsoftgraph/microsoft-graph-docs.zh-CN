---
title: hardwarePasswordInfo 资源类型
description: Intune 将为客户提供在已注册的 windows 10 和已加入Azure Active Directory配置硬件/bios 设置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7fd663fbcfd721e6fd6ed762d0de2b107503ec2c
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61345417"
---
# <a name="hardwarepasswordinfo-resource-type"></a>hardwarePasswordInfo 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Intune 将为客户提供在已注册的 windows 10 和已加入Azure Active Directory配置硬件/bios 设置。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 hardwarePasswordInfos](../api/intune-deviceconfig-hardwarepasswordinfo-list.md)|[hardwarePasswordInfo](../resources/intune-deviceconfig-hardwarepasswordinfo.md) 集合|列出 [hardwarePasswordInfo](../resources/intune-deviceconfig-hardwarepasswordinfo.md) 对象的属性和关系。|
|[获取 hardwarePasswordInfo](../api/intune-deviceconfig-hardwarepasswordinfo-get.md)|[hardwarePasswordInfo](../resources/intune-deviceconfig-hardwarepasswordinfo.md)|读取 [hardwarePasswordInfo 对象的属性和](../resources/intune-deviceconfig-hardwarepasswordinfo.md) 关系。|
|[创建 hardwarePasswordInfo](../api/intune-deviceconfig-hardwarepasswordinfo-create.md)|[hardwarePasswordInfo](../resources/intune-deviceconfig-hardwarepasswordinfo.md)|创建新的 [hardwarePasswordInfo](../resources/intune-deviceconfig-hardwarepasswordinfo.md) 对象。|
|[删除 hardwarePasswordInfo](../api/intune-deviceconfig-hardwarepasswordinfo-delete.md)|None|删除 [hardwarePasswordInfo](../resources/intune-deviceconfig-hardwarepasswordinfo.md)。|
|[更新 hardwarePasswordInfo](../api/intune-deviceconfig-hardwarepasswordinfo-update.md)|[hardwarePasswordInfo](../resources/intune-deviceconfig-hardwarepasswordinfo.md)|更新 [hardwarePasswordInfo 对象](../resources/intune-deviceconfig-hardwarepasswordinfo.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|硬件密码信息的唯一标识符|
|serialNumber|String|设备序列号|
|currentPassword|String|当前设备密码|
|previousPasswords|String collection|以前的设备密码列表|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.hardwarePasswordInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwarePasswordInfo",
  "id": "String (identifier)",
  "serialNumber": "String",
  "currentPassword": "String",
  "previousPasswords": [
    "String"
  ]
}
```




