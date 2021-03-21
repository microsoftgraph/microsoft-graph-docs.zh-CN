---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d508a2ee46e5d342f01e55223d8f3f9bfb394d8c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960016"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.chats("19:ea28e88c00e94c7786b065394a61f296@thread.v2").installedApps("NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=")
    .upgrade()
    .buildRequest()
    .post();

```