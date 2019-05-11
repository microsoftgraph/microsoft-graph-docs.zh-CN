---
title: appLogUploadState 枚举类型
description: AppLogUploadStatus
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c6a0c880fe8fa7fe743bea3ad42fee6d1e24d209
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943114"
---
# <a name="apploguploadstate-enum-type"></a>appLogUploadState 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

AppLogUploadStatus

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|决|0|请求正在等待处理或在处理|
|后|1|请求已完成, 且文件已上载到 Azure blob 以供下载。|
|未能|双面|请求已完成处理且处于错误状态。|




