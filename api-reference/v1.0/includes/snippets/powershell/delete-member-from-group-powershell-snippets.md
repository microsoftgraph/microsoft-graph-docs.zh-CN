---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49aa2f46f3991d29cded9964d5a224217f142072
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439290"
---
```powershell

Import-Module Microsoft.Graph.Groups

Remove-MgGroupMemberByRef -GroupId $groupId -DirectoryObjectId $directoryObjectId

```