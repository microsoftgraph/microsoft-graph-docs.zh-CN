---
title: enrollmentState 枚举类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b71f41d459e3fdb50fd853c62a855b4591a8ca8e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419105"
---
# <a name="enrollmentstate-enum-type"></a>enrollmentState 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|设备注册状态是未知|
|注册|1|注册设备。|
|pendingReset|2|注册但它通过注册配置文件中注册的注册的配置文件是不同的已分配的配置文件。|
|failed|3|未注册，并且没有注册失败记录。|
|notContacted|4|导入但未注册设备。|
|已阻止|5|设备注册为 userless，但阻止移动到用户注册，因为应用程序安装失败。|




