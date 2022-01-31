---
title: cloudPcOrganizationSettings 资源类型
description: 表示租户的云电脑组织设置。
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 4e8cbb2e5dbf87eb34decbf3ec5161477cbd2cf1
ms.sourcegitcommit: a60e5e81cfa04b666a1df1111a1d91f6c11989e9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2022
ms.locfileid: "62282152"
---
# <a name="cloudpcorganizationsettings-resource-type"></a>cloudPcOrganizationSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户的云电脑组织设置。 租户只有一个 **cloudPcOrganizationSettings** 对象。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 cloudPcOrganizationSettings](../api/cloudpcorganizationsettings-get.md)|[cloudPcOrganizationSettings](../resources/cloudpcorganizationsettings.md)|读取 [cloudPcOrganizationSettings 对象的属性和](../resources/cloudpcorganizationsettings.md) 关系。|
|[更新 cloudPcOrganizationSettings](../api/cloudpcorganizationsettings-update.md)|[cloudPcOrganizationSettings](../resources/cloudpcorganizationsettings.md)|更新 [cloudPcOrganizationSettings 对象](../resources/cloudpcorganizationsettings.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|组织设置的 ID。|
|osVersion|[cloudPcOperatingSystem](#cloudpcoperatingsystem-values)|操作系统版本 (操作系统) 在云 PC 上预配。 可能的值包括 `windows10`、`windows11`、`unknownFutureValue`。|
|userAccountType|[cloudPcUserAccountType](#cloudpcuseraccounttype-values)|已预配云 PC 上的用户的帐户类型。 可能的值包括 `standardUser`、`administrator`、`unknownFutureValue`。|

### <a name="cloudpcoperatingsystem-values"></a>cloudPcOperatingSystem 值

|成员|说明|
|:---|:---|
|windows10|Windows 10操作系统。|
|windows11|Windows 11操作系统。|
|unknownFutureValue|可发展枚举 sentinel 值。 请勿使用。|

### <a name="cloudpcuseraccounttype-values"></a>cloudPcUserAccountType 值

|成员|说明|
|:---|:---|
|standardUser|在云电脑上没有本地管理权限的用户。 标准用户只能安装来自 Microsoft Store 的内容，但他们无法Windows需要本地管理权限的自定义设置。|
|administrator|在云电脑上具有完全本地管理权限的用户。 管理员可以在云电脑上安装任何软件并修改任何文件或设置。|
|unknownFutureValue|可发展枚举 sentinel 值。 请勿使用。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcOrganizationSettings",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcOrganizationSettings",
  "id": "String (identifier)",
  "osVersion": "String",
  "userAccountType": "String"
}
```
