---
title: mobileAppSupersedenceType 枚举类型
description: 指示与两个移动应用程序之间的关系相关联的取代类型。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 91629d4effbda6077eb3c12db62417becbdaf609
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129059"
---
# <a name="mobileappsupersedencetype-enum-type"></a>mobileAppSupersedenceType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指示与两个移动应用程序之间的关系相关联的取代类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|update|0|指示子应用应按父应用的内部逻辑进行更新。|
|replace|1|指示在安装父应用之前应卸载子应用。|



