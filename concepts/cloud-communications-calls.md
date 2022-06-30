---
title: 云通信 API 中支持的呼叫类型
description: 了解 Microsoft Graph 中云通信 API 中支持的调用类型，以及它们如何用于信号过程。
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.openlocfilehash: 21b220b75e4d78286a7455fc042066ca50b67c45
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441018"
---
# <a name="supported-call-types"></a>支持的呼叫类型

本文介绍 Microsoft Graph 中云通信 API 中支持的调用类型，以及它们如何用于信号过程。

## <a name="peer-to-peer-calls"></a>对等调用

当一个参与者直接调用另一个参与者时，呼叫是对等 (P2P) 。 如果机器人调用用户，并且用户是唯一指定的调用目标，则这是 P2P 调用的示例。

![P2P 调用关系图](images/communications-p2p-call.PNG)

如果用户想要调用机器人，则机器人不需要任何其他权限来响应 P2P 调用。 为了使机器人调用用户，它必须具有 P2P 调用的 Call.Initiate.All 权限。

## <a name="group-calls"></a>组调用

如果呼叫中有三个或多个参与者，或者在最初创建呼叫时指定了 [会议坐标](/graph/api/resources/onlinemeeting) ，则会发生组呼叫。 

例如，可以通过 Microsoft Teams 创建组调用。

![组调用图](images/communications-group-call.PNG)

目前，机器人能够：
- 创建组调用
- 加入排泄组调用
- 邀请其他参与者加入现有组调用
- 受邀加入现有组调用

## <a name="see-also"></a>另请参阅

- [云通信 API 概述](cloud-communications-concept-overview.md)
- [调用的权限](./permissions-reference.md#calls-permissions)
