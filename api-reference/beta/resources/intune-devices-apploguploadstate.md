---
title: appLogUploadState 枚举类型
description: AppLogUploadStatus
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ca37de06d50f57eda6c094f195fb5f291181034a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337585"
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



