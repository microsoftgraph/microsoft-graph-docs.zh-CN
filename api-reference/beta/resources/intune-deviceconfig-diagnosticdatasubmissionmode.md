---
title: diagnosticDataSubmissionMode 枚举类型
description: 允许设备发送诊断和使用情况遥测数据，例如 Watson。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 42da759552f2e9a4137fb27ec90e399053f1b3f753e68f92e66f077702ed4774
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54124771"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>diagnosticDataSubmissionMode 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

允许设备发送诊断和使用情况遥测数据，例如 Watson。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|userDefined|0|允许用户设置。|
|无|1 |不会从操作系统组件发送遥测数据。 注意：此值仅适用于企业和服务器设备。 在其他设备上使用此设置等效于将值设置为 1。|
|basic|2 |发送基本遥测数据。|
|增强|3 |发送增强的遥测数据，包括使用情况和见解数据。|
|full|4 |发送完整的遥测数据，包括诊断数据，如系统状态。|




