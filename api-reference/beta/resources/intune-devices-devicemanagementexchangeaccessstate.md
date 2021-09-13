---
title: deviceManagementExchangeAccessState 枚举类型
description: 设备Exchange访问状态。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 75d24d4a5802a79f6fbfecdb4970e035618d08ea
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59144208"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a>deviceManagementExchangeAccessState 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备Exchange访问状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|未从用户发现任何Exchange|
|unknown|1|设备访问状态Exchange未知|
|allowed|2|设备有权访问Exchange|
|blocked|3|设备在Exchange|
|quarantined|4 |设备已隔离Exchange|



