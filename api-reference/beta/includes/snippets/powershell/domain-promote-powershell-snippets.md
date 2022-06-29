---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19ee47eaf1bd454650972ffe4a7555d5eb1ec2e1
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446626"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Invoke-MgPromoteDomain -DomainId $domainId

```