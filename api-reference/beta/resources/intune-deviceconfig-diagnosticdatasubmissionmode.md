---
title: diagnosticDataSubmissionMode 枚举类型
description: 允许设备发送诊断和使用遥测数据, 如 Watson。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fce6bbe40d985c15c5455c3b83de88ced4cce768
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332685"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>diagnosticDataSubmissionMode 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

允许设备发送诊断和使用遥测数据, 如 Watson。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|定制|0|允许用户进行设置。|
|无|1|不会从 OS 组件发送遥测数据。 注意: 此值仅适用于企业和服务器设备。 在其他设备上使用此设置等效于将值设置为1。|
|vba|双面|发送基本遥测数据。|
|有所|第三章|发送包含使用率和见解数据的增强遥测数据。|
|全|4|发送包含诊断数据 (如系统状态) 的完整遥测数据。|



