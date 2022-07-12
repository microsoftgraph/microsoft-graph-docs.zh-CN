---
title: diagnosticDataSubmissionMode 枚举类型
description: 允许设备发送诊断和使用情况遥测数据，如 Watson。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4befef2c9a4e447869a989aad27ddb5ca1641c44
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66735115"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>diagnosticDataSubmissionMode 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

允许设备发送诊断和使用情况遥测数据，如 Watson。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|userDefined|0|允许用户设置。|
|无|1|不会从 OS 组件发送遥测数据。 注意：此值仅适用于企业和服务器设备。 在其他设备上使用此设置等效于设置值 1。|
|基本|2|发送基本遥测数据。|
|增强|3|发送增强的遥测数据，包括使用情况和见解数据。|
|全|4|发送完整的遥测数据，包括诊断数据，如系统状态。|





