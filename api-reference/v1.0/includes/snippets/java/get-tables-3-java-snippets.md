---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 544a5e154f763d5263279f46e98b9a26d63e89b7
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209382"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookTableCollectionPage tables = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").tables()
    .buildRequest()
    .get();

```