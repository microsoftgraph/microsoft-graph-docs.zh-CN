---
title: vppTokenSyncStatus 枚举类型
description: 与 Apple Volume Purchase Program 令牌关联的可能同步状态。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d6149d596b4a44d10585d34559af8e400597d1ea
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59101175"
---
# <a name="vpptokensyncstatus-enum-type"></a>vppTokenSyncStatus 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

与 Apple Volume Purchase Program 令牌关联的可能同步状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|默认状态。|
|inProgress|1|正在同步的最后一个同步。|
|已完成|2|上次同步成功完成。|
|failed|3|上次同步失败。|



