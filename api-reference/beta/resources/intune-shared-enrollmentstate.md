---
title: enrollmentState 枚举类型
description: 尚未记录
author: rolyon
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f06cb39e94dd526368b237b04d0bfefd9d68d095
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046608"
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
|enrolled|1|设备已注册。|
|pendingReset|2|已注册，但通过注册配置文件注册，并且已注册的配置文件与分配的配置文件不同。|
|failed|3|未注册，并且存在注册失败记录。|
|notContacted|4 |设备已导入，但没有注册。|
|blocked|5 |设备以无用户状态注册，但因应用安装失败，无法移动到用户注册。|



