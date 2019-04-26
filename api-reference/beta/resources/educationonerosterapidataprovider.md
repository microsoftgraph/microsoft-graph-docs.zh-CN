---
title: educationOneRosterApiDataProvider 资源
description: 用于在将 OneRoster API 用作输入源时设置学校数据同步配置文件。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 4ac232f71600f701efd8d085386fa9070773b475
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334183"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="6f7c0-103">educationOneRosterApiDataProvider 资源</span><span class="sxs-lookup"><span data-stu-id="6f7c0-103">educationOneRosterApiDataProvider resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f7c0-104">用于在将[OneRoster API](https://www.imsglobal.org/activity/onerosterlis)用作输入源时设置学校数据同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="6f7c0-104">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="6f7c0-105">派生自[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="6f7c0-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6f7c0-106">属性</span><span class="sxs-lookup"><span data-stu-id="6f7c0-106">Properties</span></span>

| <span data-ttu-id="6f7c0-107">属性</span><span class="sxs-lookup"><span data-stu-id="6f7c0-107">Property</span></span> | <span data-ttu-id="6f7c0-108">类型</span><span class="sxs-lookup"><span data-stu-id="6f7c0-108">Type</span></span> | <span data-ttu-id="6f7c0-109">说明</span><span class="sxs-lookup"><span data-stu-id="6f7c0-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="6f7c0-110">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="6f7c0-110">**connectionUrl**</span></span> | <span data-ttu-id="6f7c0-111">String</span><span class="sxs-lookup"><span data-stu-id="6f7c0-111">String</span></span> | <span data-ttu-id="6f7c0-112">指向 OneRoster 实例的连接 URL。</span><span class="sxs-lookup"><span data-stu-id="6f7c0-112">The connection URL to the OneRoster instance.</span></span> |
| <span data-ttu-id="6f7c0-113">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="6f7c0-113">**schoolsIds**</span></span> | <span data-ttu-id="6f7c0-114">String 集合</span><span class="sxs-lookup"><span data-stu-id="6f7c0-114">String collection</span></span> |  <span data-ttu-id="6f7c0-115">要同步的学校 sourcedIds 的列表。</span><span class="sxs-lookup"><span data-stu-id="6f7c0-115">The list of school sourcedIds to sync.</span></span> |
| <span data-ttu-id="6f7c0-116">**providerName**</span><span class="sxs-lookup"><span data-stu-id="6f7c0-116">**providerName**</span></span> | <span data-ttu-id="6f7c0-117">String</span><span class="sxs-lookup"><span data-stu-id="6f7c0-117">String</span></span> | <span data-ttu-id="6f7c0-118">由[OneRoster 规范](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA)定义的 OneRoster 服务提供程序名称。</span><span class="sxs-lookup"><span data-stu-id="6f7c0-118">The OneRoster Service Provider name as defined by the [OneRoster specification](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span></span> |
| <span data-ttu-id="6f7c0-119">**connectionSettings**</span><span class="sxs-lookup"><span data-stu-id="6f7c0-119">**connectionSettings**</span></span> | [<span data-ttu-id="6f7c0-120">educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="6f7c0-120">microsoft.graph.educationSynchronizationConnectionSettings</span></span>](educationsynchronizationconnectionsettings.md) | <span data-ttu-id="6f7c0-121">OneRoster 实例的连接设置。</span><span class="sxs-lookup"><span data-stu-id="6f7c0-121">Connection settings for the OneRoster instance.</span></span> <span data-ttu-id="6f7c0-122">应为[educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md)或[educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md)的类型类型。</span><span class="sxs-lookup"><span data-stu-id="6f7c0-122">Should be of type [microsoft.graph.educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) or [microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span></span> |
| <span data-ttu-id="6f7c0-123">**操作**</span><span class="sxs-lookup"><span data-stu-id="6f7c0-123">**customizations**</span></span> | [<span data-ttu-id="6f7c0-124">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="6f7c0-124">microsoft.graph.educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="6f7c0-125">要应用于同步配置文件的可选自定义项。</span><span class="sxs-lookup"><span data-stu-id="6f7c0-125">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6f7c0-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6f7c0-126">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider",
    "connectionUrl": "String",
    "providerName": "String",
    "schoolsIds": [
        "String"
    ],
    "connectionSettings": {
        "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
        "clientId": "String",
        "clientSecret": "String",
    },
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
