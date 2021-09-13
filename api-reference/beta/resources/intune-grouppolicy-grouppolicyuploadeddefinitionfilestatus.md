---
title: groupPolicyUploadedDefinitionFileStatus 枚举类型
description: 组策略上载的定义文件状态的类型。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 765300d2af833a2dfaa8e6b42aac47281da01d1f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59030184"
---
# <a name="grouppolicyuploadeddefinitionfilestatus-enum-type"></a>groupPolicyUploadedDefinitionFileStatus 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

组策略上载的定义文件状态的类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|组策略上载的定义文件上传状态无效。|
|uploadInProgress|1|正在上载组策略上载的定义文件。|
|可用|2|组策略上载的定义文件可用。|
|已分配|3|分配给策略的组策略上载的定义文件。|
|removalInProgress|4 |正在删除组策略上载的定义文件。|
|uploadFailed|5 |组策略上载的定义文件上传失败。|
|removalFailed|6 |组策略上载的定义文件删除失败。|



