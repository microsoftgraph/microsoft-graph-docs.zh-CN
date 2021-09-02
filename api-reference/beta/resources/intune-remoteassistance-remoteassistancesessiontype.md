---
title: remoteAssistanceSessionType 枚举类型
description: 已召开的远程协助会话的类型。 可能的值包括： `viewOnly` 、 `fullControl`
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4aea876b672a71e9bc82e9eea620d257c3c5ea01
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58794300"
---
# <a name="remoteassistancesessiontype-enum-type"></a>remoteAssistanceSessionType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

已召开的远程协助会话的类型。 可能的值包括： `viewOnly` 、 `fullControl`

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|viewOnly|0|此状态表示帮助程序与共享者之间的仅查看会话。|
|fullControl|1|此状态表示帮助程序能够完全控制共享者设备的会话。|
|elevation|2|此状态表示帮助程序能够在共享者设备上执行管理操作的会话。|



