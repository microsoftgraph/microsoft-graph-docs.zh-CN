---
title: enrollmentState 枚举类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0817bb82e098d1fab93da3381c81faafc03b4cf0810e602934924305e0971edf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54206107"
---
# <a name="enrollmentstate-enum-type"></a>enrollmentState 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|设备注册状态未知|
|enrolled|1 |设备已注册。|
|pendingReset|2 |已注册，但通过注册配置文件注册，并且已注册的配置文件与分配的配置文件不同。|
|failed|3 |未注册，并且存在注册失败记录。|
|notContacted|4 |设备已导入，但没有注册。|
|blocked|5 |设备以无用户状态注册，但因应用安装失败，无法移动到用户注册。|




