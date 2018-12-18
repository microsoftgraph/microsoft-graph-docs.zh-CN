---
title: appListType 枚举类型
description: 合规性应用程序列表的可能值。
author: tfitzmac
ms.openlocfilehash: ab5d8f45343b017693906b13be25c88d5b06e8f7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354717"
---
# <a name="applisttype-enum-type"></a>appListType 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

合规性应用程序列表的可能值。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|默认值，没有用途。|
|appsInListCompliant|1|在列表代表将被视为符合 （仅在列表上的应用程序都符合） 的应用程序。|
|appsNotInListCompliant|2|在列表代表将被视为不符合标准的应用程序 （所有应用程序是除列表上的应用程序兼容）。|



