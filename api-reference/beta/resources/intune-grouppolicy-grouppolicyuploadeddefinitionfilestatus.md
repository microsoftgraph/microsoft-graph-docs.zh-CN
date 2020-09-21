---
title: groupPolicyUploadedDefinitionFileStatus 枚举类型
description: 组策略上载的定义文件状态的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 70430e74d332baf0b1c81a41d2098883688464ea
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030610"
---
# <a name="grouppolicyuploadeddefinitionfilestatus-enum-type"></a>groupPolicyUploadedDefinitionFileStatus 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

组策略上载的定义文件状态的类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|组策略上传的定义文件上载状态无效。|
|uploadInProgress|1 |组策略上传的定义文件上载正在进行中。|
|可用|2 |组策略已上载的定义文件可用。|
|赋予|第三章|组策略已上载分配给策略的定义文件。|
|removalInProgress|4 |组策略上传的定义文件正在删除。|
|uploadFailed|5 |组策略上载的定义文件上载失败。|
|removalFailed|6 |组策略上传的定义文件删除失败。|






