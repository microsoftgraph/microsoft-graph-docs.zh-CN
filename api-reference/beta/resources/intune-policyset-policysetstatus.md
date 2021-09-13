---
title: policySetStatus 枚举类型
description: 用于指定 PolicySet 状态的枚举。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 22091444272c3e88648e1e14483ec58ce6f78873
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59020320"
---
# <a name="policysetstatus-enum-type"></a>policySetStatus 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于指定 PolicySet 状态的枚举。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|默认值。|
|验证|1|所有 PolicySet 项现在都验证工作负荷的相应设置。|
|partialSuccess|2|完成所有 PolicySet 项的进程后，但失败。|
|success|3|部署所有 PolicySet 项。 并不意味着所有部署都成功。 |
|error|4 |PolicySet 处理完全失败。|
|notAssigned|5 |未向任何组分配 PolicySet/PolicySetItem。|



