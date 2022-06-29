---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13af83bc19e04020e65602a1babae6d9c39dfed9
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442206"
---
```powershell

Import-Module Microsoft.Graph.Groups

Remove-MgGroupOwnerByRef -GroupId $groupId -DirectoryObjectId $directoryObjectId

```