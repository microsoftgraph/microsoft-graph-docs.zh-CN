---
title: groupPolicyUploadedDefinitionFileStatus 枚举类型
description: 组策略上载的定义文件状态的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 49a0bde51eb726b72c1978d5323f9c6699895d80
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58784777"
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



