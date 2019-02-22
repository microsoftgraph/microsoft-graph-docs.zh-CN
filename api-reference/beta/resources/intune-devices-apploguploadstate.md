---
title: appLogUploadState 枚举类型
description: AppLogUploadStatus
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8f8243436fa9ec5a56f442626cea31819ca1eaef
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174387"
---
# <a name="apploguploadstate-enum-type"></a>appLogUploadState 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

AppLogUploadStatus

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|决|0|请求正在等待处理或在处理|
|后|1|请求已完成, 且文件已上载到 Azure blob 以供下载。|
|failed|双面|请求已完成处理且处于错误状态。|




