---
title: educationSynchronizationConnectionSettings 资源类型
description: '代表提供商连接设置。 这样，系统知道如何连接到提供程序的 Api。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f9bb19ec9c09b06dd007eb2031f3dbb176eb12d3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978226"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="bbb5e-104">educationSynchronizationConnectionSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="bbb5e-104">educationSynchronizationConnectionSettings resource type</span></span>

> <span data-ttu-id="bbb5e-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bbb5e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bbb5e-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bbb5e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bbb5e-107">代表提供商连接设置。</span><span class="sxs-lookup"><span data-stu-id="bbb5e-107">Represents the provider connection settings.</span></span> <span data-ttu-id="bbb5e-108">这样，系统知道如何连接到提供程序的 Api。</span><span class="sxs-lookup"><span data-stu-id="bbb5e-108">This allows the system to know how to connect to the provider APIs.</span></span> 

> <span data-ttu-id="bbb5e-109">**注意：** 此复杂类型是抽象类。</span><span class="sxs-lookup"><span data-stu-id="bbb5e-109">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="bbb5e-110">引用的特定类型的列出的连接设置。</span><span class="sxs-lookup"><span data-stu-id="bbb5e-110">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="bbb5e-111">派生的类型</span><span class="sxs-lookup"><span data-stu-id="bbb5e-111">Derived types</span></span>
| <span data-ttu-id="bbb5e-112">类型</span><span class="sxs-lookup"><span data-stu-id="bbb5e-112">Type</span></span> | <span data-ttu-id="bbb5e-113">说明</span><span class="sxs-lookup"><span data-stu-id="bbb5e-113">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="bbb5e-114">**educationSynchronizationOAuth1ConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="bbb5e-114">**educationSynchronizationOAuth1ConnectionSettings**</span></span>](educationsynchronizationoauth1connectionsettings.md) | <span data-ttu-id="bbb5e-115">使用此类型提供 OAuth1 连接设置。</span><span class="sxs-lookup"><span data-stu-id="bbb5e-115">Use this type to provide OAuth1 connection settings.</span></span> |
| [<span data-ttu-id="bbb5e-116">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="bbb5e-116">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="bbb5e-117">使用此类型提供 OAuth2 客户端凭据授予连接设置。</span><span class="sxs-lookup"><span data-stu-id="bbb5e-117">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="bbb5e-118">属性</span><span class="sxs-lookup"><span data-stu-id="bbb5e-118">Properties</span></span>

| <span data-ttu-id="bbb5e-119">属性</span><span class="sxs-lookup"><span data-stu-id="bbb5e-119">Property</span></span> | <span data-ttu-id="bbb5e-120">类型</span><span class="sxs-lookup"><span data-stu-id="bbb5e-120">Type</span></span> | <span data-ttu-id="bbb5e-121">说明</span><span class="sxs-lookup"><span data-stu-id="bbb5e-121">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="bbb5e-122">**clientId**</span><span class="sxs-lookup"><span data-stu-id="bbb5e-122">**clientId**</span></span> | <span data-ttu-id="bbb5e-123">字符串</span><span class="sxs-lookup"><span data-stu-id="bbb5e-123">String</span></span> |  <span data-ttu-id="bbb5e-124">用于连接到提供程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="bbb5e-124">Client ID used to connect to the provider.</span></span> |
| <span data-ttu-id="bbb5e-125">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="bbb5e-125">**clientSecret**</span></span> | <span data-ttu-id="bbb5e-126">字符串</span><span class="sxs-lookup"><span data-stu-id="bbb5e-126">String</span></span> |  <span data-ttu-id="bbb5e-127">验证连接到提供程序的客户端机密。</span><span class="sxs-lookup"><span data-stu-id="bbb5e-127">Client secret to authenticate the connection to the provider.</span></span> |
