---
title: actionState 枚举类型
description: 设备上操作的状态
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c23caa7638054d50cd12c0081312f534d37f06bf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039306"
---
# <a name="actionstate-enum-type"></a>actionState 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备上操作的状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|操作状态无效|
|pending|1|操作挂起|
|canceled|2|操作已取消。|
|active|3|操作处于活动状态。|
|done|4 |操作已完成，没有错误。|
|failed|5 |操作失败|
|notSupported|6 |不支持操作。|



