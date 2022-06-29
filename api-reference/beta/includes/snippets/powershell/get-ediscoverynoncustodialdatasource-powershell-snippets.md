---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca92fabeadc1a80201ae41c581abc528ba4290d3
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66438734"
---
```powershell

Import-Module Microsoft.Graph.Security

Get-MgSecurityCaseEdiscoveryCaseNoncustodialDataSource -EdiscoveryCaseId $ediscoveryCaseId -EdiscoveryNoncustodialDataSourceId $ediscoveryNoncustodialDataSourceId -ExpandProperty "dataSource" 

```