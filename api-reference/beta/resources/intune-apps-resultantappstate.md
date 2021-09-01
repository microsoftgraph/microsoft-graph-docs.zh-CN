---
title: resultantAppState 枚举类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 90f8e3dd14ac09945e5f21d8ccee9d2df214ef09
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58790442"
---
# <a name="resultantappstate-enum-type"></a>resultantAppState 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|已安装|1|安装应用程序时没有出现错误|
|failed|2|应用程序安装失败。|
|notInstalled|3|未安装应用程序。|
|uninstallFailed|4 |应用程序无法卸载。|
|pendingInstall|5 |应用程序安装正在进行中。|
|unknown|99|应用程序的状态未知。|
|notApplicable|-1|应用程序不适用。|



