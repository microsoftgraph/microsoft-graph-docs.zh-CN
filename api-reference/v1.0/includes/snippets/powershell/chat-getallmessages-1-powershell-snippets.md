---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf82870748679978d9d5767d330e8fde38448abc
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66502566"
---
```powershell

Import-Module Microsoft.Graph.Users.Functions

Get-MgAllUserChatMessage -UserId $userId -Top 2 

```