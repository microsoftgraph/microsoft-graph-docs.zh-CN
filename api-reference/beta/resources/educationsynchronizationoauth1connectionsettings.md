---
title: educationSynchronizationOAuth1ConnectionSettings 资源
description: 当 OAuth1 用于连接到数据提供程序时，此连接设置类型应用于设置配置文件。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 525809121b07616c6eb5077f1b12d5b736586065
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434919"
---
# <a name="educationsynchronizationoauth1connectionsettings-resource"></a><span data-ttu-id="da305-103">educationSynchronizationOAuth1ConnectionSettings 资源</span><span class="sxs-lookup"><span data-stu-id="da305-103">educationSynchronizationOAuth1ConnectionSettings resource</span></span>

<span data-ttu-id="da305-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da305-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da305-105">当 OAuth1 用于连接到数据提供程序时，此连接设置类型应用于设置配置文件。</span><span class="sxs-lookup"><span data-stu-id="da305-105">When OAuth1 is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="da305-106">派生自[educationSynchronizationConnectionSettings]。</span><span class="sxs-lookup"><span data-stu-id="da305-106">Derived from [educationSynchronizationConnectionSettings].</span></span>

## <a name="properties"></a><span data-ttu-id="da305-107">属性</span><span class="sxs-lookup"><span data-stu-id="da305-107">Properties</span></span>

| <span data-ttu-id="da305-108">属性</span><span class="sxs-lookup"><span data-stu-id="da305-108">Property</span></span>     | <span data-ttu-id="da305-109">类型</span><span class="sxs-lookup"><span data-stu-id="da305-109">Type</span></span>   | <span data-ttu-id="da305-110">说明</span><span class="sxs-lookup"><span data-stu-id="da305-110">Description</span></span>                                                                                                                |
| :----------- | :----- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="da305-111">clientId</span><span class="sxs-lookup"><span data-stu-id="da305-111">clientId</span></span>     | <span data-ttu-id="da305-112">字符串</span><span class="sxs-lookup"><span data-stu-id="da305-112">String</span></span> | <span data-ttu-id="da305-113">用于连接到提供程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="da305-113">Client ID used to connect to the provider.</span></span> <span data-ttu-id="da305-114">继承自[educationSynchronizationConnectionSettings]。</span><span class="sxs-lookup"><span data-stu-id="da305-114">Inherited from [educationSynchronizationConnectionSettings].</span></span>                    |
| <span data-ttu-id="da305-115">clientSecret</span><span class="sxs-lookup"><span data-stu-id="da305-115">clientSecret</span></span> | <span data-ttu-id="da305-116">字符串</span><span class="sxs-lookup"><span data-stu-id="da305-116">String</span></span> | <span data-ttu-id="da305-117">用于对与提供程序的连接进行身份验证的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="da305-117">Client secret to authenticate the connection to the provider.</span></span> <span data-ttu-id="da305-118">继承自[educationSynchronizationConnectionSettings]。</span><span class="sxs-lookup"><span data-stu-id="da305-118">Inherited from [educationSynchronizationConnectionSettings].</span></span> |

[educationsynchronizationconnectionsettings]: educationsynchronizationconnectionsettings.md

## <a name="json-representation"></a><span data-ttu-id="da305-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="da305-120">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
  "clientId": "String",
  "clientSecret": "String"
}
```
