---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42468d9365203acff43a4a80fd8299946c20d2a4
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519459"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SetCollectionPage sets = graphClient.sites("microsoft.sharepoint.com,b9b0bc03-cbc4-40d2-aba9-2c9dd9821ddf,6a742cee-9216-4db5-8046-13a595684e74").termStore().groups("03577abb-975e-4fb4-9ee0-4102a9108f94").sets()
    .buildRequest()
    .get();

```