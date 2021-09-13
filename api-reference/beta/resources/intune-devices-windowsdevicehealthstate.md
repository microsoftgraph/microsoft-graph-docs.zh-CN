---
title: windowsDeviceHealthState 枚举类型
description: 计算机终结点保护状态
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5fe5692a8d694076cc060f2c21164fe6a5fe25bb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59142983"
---
# <a name="windowsdevicehealthstate-enum-type"></a>windowsDeviceHealthState 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

计算机终结点保护状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|clean|0|计算机干净，无需任何操作|
|fullScanPending|1|计算机正等待完全扫描状态|
|rebootPending|2|计算机正等待重启状态|
|manualStepsPending|4 |计算机正等待手动步骤状态|
|offlineScanPending|8 |计算机处于挂起脱机扫描状态|
|critical|16 |计算机正发生严重故障状态|



