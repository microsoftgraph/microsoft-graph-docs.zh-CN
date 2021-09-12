---
title: win32LobAppFileSystemOperationType 枚举类型
description: 包含所有受支持的文件系统检测类型。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: cd46b79237c25bfd0974e25f0fc8908ed46389d0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59017567"
---
# <a name="win32lobappfilesystemoperationtype-enum-type"></a>win32LobAppFileSystemOperationType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含所有受支持的文件系统检测类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未配置。|
|exists|1|指定的文件或文件夹是否存在。|
|modifiedDate|2|上次修改日期。|
|createdDate|3|创建日期。|
|version|4 |版本值类型。|
|sizeInMB|5 |大小检测类型。|
|doesNotExist|6 |指定的文件或文件夹不存在。|



