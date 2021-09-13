---
title: 呼叫概述
description: 了解受支持的呼叫类型以及如何将这些类型用于信号过程。
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.openlocfilehash: 34b7e2e507576333df36f7eae9185785872d24ec
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59137488"
---
# <a name="calls-overview"></a>呼叫概述

Microsoft 中的云通信 API Graph通过各种通信相关功能（如呼叫和联机会议）为应用和服务如何与用户交互添加了新的维度。 本文介绍支持的呼叫类型以及如何将这些类型用于信号过程。

## <a name="peer-to-peer-calls"></a>对等呼叫
当一个参与者直接呼叫另一个 (时，呼叫) P2P 呼叫。 如果机器人呼叫用户，并且该用户是唯一指定的呼叫目标，则这是 P2P 呼叫的一个示例。

![P2P 呼叫图](images/communications-p2p-call.PNG)

如果用户想要呼叫机器人，则机器人不需要任何其他权限来响应 P2P 呼叫。 若要使机器人呼叫用户，它必须具有Calls.Ini平铺。P2P 调用的所有权限。

## <a name="group-calls"></a>组内呼叫

如果呼叫有三个或三个以上参与者，或者最初创建呼叫时指定了会议坐标，[](/graph/api/resources/onlinemeeting)则会发生群组呼叫。 

例如，可以通过 Microsoft Teams 创建组呼叫。

![组呼叫图](images/communications-group-call.PNG)

目前，机器人能够：
- 创建组呼叫
- 加入 exisiting 组呼叫
- 邀请其他参与者加入现有组通话
- 受邀加入现有组呼叫

## <a name="see-also"></a>另请参阅

- [云通信 API 概述](cloud-communications-concept-overview.md)
- [呼叫权限](./permissions-reference.md#calls-permissions)
