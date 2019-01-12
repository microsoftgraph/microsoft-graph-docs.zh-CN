---
title: appListType 枚举类型
description: 合规性应用程序列表的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: eb2b4afa6639d70b81a59bda1250ea9ed231ccdb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939642"
---
# <a name="applisttype-enum-type"></a>appListType 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

合规性应用程序列表的可能值。
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|无|0|默认值，没有用途。|
|appsInListCompliant|1|在列表代表将被视为符合 （仅在列表上的应用程序都符合） 的应用程序。|
|appsNotInListCompliant|2|在列表代表将被视为不符合标准的应用程序 （所有应用程序是除列表上的应用程序兼容）。|





