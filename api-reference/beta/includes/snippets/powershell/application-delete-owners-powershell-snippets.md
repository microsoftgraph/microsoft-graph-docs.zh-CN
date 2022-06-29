---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4fcb1507ddcc04cceedc8656dce2ca926c65f4f9
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66438226"
---
```powershell

Import-Module Microsoft.Graph.Applications

Remove-MgApplicationOwnerByRef -ApplicationId $applicationId -DirectoryObjectId $directoryObjectId

```