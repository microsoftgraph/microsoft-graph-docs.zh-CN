---
title: Microsoft Graph 中的设备中继 API（预览版）
description: '当今，人们每天都会与多个设备进行交互。 用户通常会在一个设备上开始生产任务和娱乐活动，并在另一个设备上继续进行。 为了满足客户的各种需求，你的应用需要能够无缝跨多个设备和平台。 '
localization_priority: Normal
author: davidmu1
ms.prod: cross-device-experiences
ms.openlocfilehash: f520c90eda15c9e571deb34865fdf81dd4954d50
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952485"
---
# <a name="device-relay-api-in-microsoft-graph-preview"></a>Microsoft Graph 中的设备中继 API（预览版）

当今，人们每天都会与多个设备进行交互。 用户通常会在一个设备上开始生产任务和娱乐活动，并在另一个设备上继续进行。 为了满足客户的各种需求，你的应用需要能够无缝跨多个设备和平台。 

你可以使用设备中继 API 为用户提供无缝体验， 让他们积极地将体验从一个设备转移到另一个设备，或者一次使用多个设备提升体验。 这可以通过应用内操作（应用中的按钮或选择）来完成，通过调用设备中继 API 来发现用户设备，并使其能够在其他设备上启动和向应用发送消息。

## <a name="why-integrate-with-device-relay"></a>为什么与设备中继集成？

设备中继 API 能够让应用自行注册，并在用户设备上发现、命令应用以及向其发送消息。 通过集成，你可以将客户所处理的任务置于中心焦点。 通过发现设备并将任务转移到该设备上，客户即可在他们最为便捷的设备上继续工作。 另外，他们还可以通过使用周围的其他设备来增强应用的持续体验。

你可以将设备中继 API 用于配套设备或远程控制应用场景。 使用消息功能在两台设备之间创建应用频道以发送和接收自定义消息。 例如，可以让客户使用自己的手机控制电视的播放。 而且，当用户在 PC 上处理应用的主视图时，通过在手机上显示基于上下文的常用操作，还可以在工作效率场景中提供配套应用。

通过在应用中执行操作，客户还可以主动将体验从一个设备转移到另一个设备。 例如，某位用户在公交车上用手机在观看现场直播，但当她到家后，她可能想要转到客厅中的电脑上播放。 设备中继也支持工作效率应用场景。 

### <a name="extend-the-experience"></a>扩展体验

通过提供 UX 来发现设备并在这些设备上启动应用，从而扩展应用。 例如，用户可以在她的手机上处理采购订单，在她的办公室发现 PC，并在其上启动应用来完成采购订单输入。  

### <a name="augment-the-experience"></a>增强体验

在用户的另一个设备上为应用创建配套体验。 例如，应用可以包含 UX 以在其他设备上自启动。 在游戏中，用户可以将应用启动到有较大屏幕的设备上（例如，从 PC 到 Xbox）。 Xbox 可以呈现游戏的完整视图（第一人称视角），而屏幕较小的设备可以呈现不同的视角和附加背景（游戏关卡的顶级视角，显示玩家与对手的位置）。  

### <a name="enrich-the-experience"></a>丰富体验

为应用添加其他控制功能。 例如，从配套设备为主应用提供远程控制功能。 当用户将应用从一个设备启动到另一个设备时，目标设备可以显示完整体验（例如，设计应用中的 3D 模型），而源设备可以显示目标设备上给定应用状态的最常用操作的列表（例如旋转、调整大小、调色板）。

## <a name="see-also"></a>另请参阅

- [Microsoft Graph 中的跨设备体验](cross-device-concept-overview.md)
- [详细了解设备中继 API](/graph/api/resources/project-rome-overview?view=graph-rest-beta)
- [详细了解 Project Rome](/windows/project-rome/)