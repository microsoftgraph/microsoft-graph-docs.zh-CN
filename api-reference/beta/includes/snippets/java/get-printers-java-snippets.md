---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 920a16373311ce7b6c1d39c30ef0dd4f89e650b6914b473989ff2a3cca6821d5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279043"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrinterCollectionPage printers = graphClient.print().printers()
    .buildRequest()
    .get();

```