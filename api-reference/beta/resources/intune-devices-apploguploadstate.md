---
title: appLogUploadState 枚举类型
description: AppLogUploadStatus
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7d304c9d0b310d26eb7c4e83144c6fa1e8a9b1b5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086279"
---
# <a name="apploguploadstate-enum-type"></a>appLogUploadState 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

AppLogUploadStatus

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|pending|0|请求正在等待处理或正在处理中|
|已完成|1|请求已完成，文件上传到 Azure blob 进行下载。|
|failed|2|请求已完成处理并出现错误状态。|



