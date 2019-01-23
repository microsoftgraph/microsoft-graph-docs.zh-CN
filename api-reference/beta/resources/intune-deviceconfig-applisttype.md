---
title: appListType 枚举类型
description: 合规性应用程序列表的可能值。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cf8930136b00b7b5579ec5e7266b6a77a9a11968
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415220"
---
# <a name="applisttype-enum-type"></a>appListType 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

合规性应用程序列表的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|默认值，没有用途。|
|appsInListCompliant|1|在列表代表将被视为符合 （仅在列表上的应用程序都符合） 的应用程序。|
|appsNotInListCompliant|2|在列表代表将被视为不符合标准的应用程序 （所有应用程序是除列表上的应用程序兼容）。|




