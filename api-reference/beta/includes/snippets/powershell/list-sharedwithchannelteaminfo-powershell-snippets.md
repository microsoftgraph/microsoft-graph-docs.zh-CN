---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04e98b38ab8e30ba05d09d954aba4811cd750ae1
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212762"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamChannelShared -TeamId $teamId -ChannelId $channelId

```