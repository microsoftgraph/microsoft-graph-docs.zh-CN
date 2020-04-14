---
title: appLogUploadState 枚举类型
description: AppLogUploadStatus
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0e3f03f988f03a2e9728d9ef705283cb4d28956b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465193"
---
# <a name="apploguploadstate-enum-type"></a>appLogUploadState 枚举类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

AppLogUploadStatus

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|决|0|请求正在等待处理或在处理|
|后|1|请求已完成，且文件已上载到 Azure blob 以供下载。|
|未能|双面|请求已完成处理且处于错误状态。|



