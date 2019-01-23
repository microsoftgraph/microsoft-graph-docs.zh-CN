---
title: appLogUploadState 枚举类型
description: AppLogUploadStatus
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 58dcc0d4a15370d6449772d917e8994f0eb9e7bd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431396"
---
# <a name="apploguploadstate-enum-type"></a>appLogUploadState 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

AppLogUploadStatus

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|挂起|0|正在等待处理请求或将其在处理|
|完成|1|文件上载到下载 Azure blob 完成请求。|
|failed|2|请求完成处理和错误状态。|




