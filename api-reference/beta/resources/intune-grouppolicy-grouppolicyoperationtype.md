---
title: groupPolicyOperationType 枚举类型
description: 组策略操作的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 573d4a492c20eb191661d00cdd2df4337a0e6703de96c696b931eefc4c18f91f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54227307"
---
# <a name="grouppolicyoperationtype-enum-type"></a>groupPolicyOperationType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

组策略操作的类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|组策略无效的操作类型。|
|upload|1 |组策略上载操作类型。|
|uploadNewVersion|2 |组策略上载新版本操作类型。|
|addLanguageFiles|3 |组策略将新语言 (ADML) 文件操作类型。|
|removeLanguageFiles|4 |组策略删除 ADML (操作) 语言。|
|updateLanguageFiles|5 |组策略更新语言 (ADML) 文件操作类型。|
|remove|6 |组策略删除上载的文件操作类型。|




