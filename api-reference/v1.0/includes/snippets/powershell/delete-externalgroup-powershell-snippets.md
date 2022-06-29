---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cdf0adc0e8cda470a309b4e3db6d96c6c35f176a
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446280"
---
```powershell

Import-Module Microsoft.Graph.Search

Remove-MgExternalConnectionGroup -ExternalConnectionId $externalConnectionId -ExternalGroupId $externalGroupId

```