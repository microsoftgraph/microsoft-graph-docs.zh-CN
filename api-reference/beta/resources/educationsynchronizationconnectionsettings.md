---
title: educationSynchronizationConnectionSettings 资源类型
description: '代表提供商连接设置。 这样，系统知道如何连接到提供程序的 Api。 '
author: mmast-msft
ms.openlocfilehash: 4e8b62a46fa6d14508a9d57ffedc46411910433d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350622"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="169e4-104">educationSynchronizationConnectionSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="169e4-104">educationSynchronizationConnectionSettings resource type</span></span>

> <span data-ttu-id="169e4-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="169e4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="169e4-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="169e4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="169e4-107">代表提供商连接设置。</span><span class="sxs-lookup"><span data-stu-id="169e4-107">Represents the provider connection settings.</span></span> <span data-ttu-id="169e4-108">这样，系统知道如何连接到提供程序的 Api。</span><span class="sxs-lookup"><span data-stu-id="169e4-108">This allows the system to know how to connect to the provider APIs.</span></span> 

> <span data-ttu-id="169e4-109">**注意：** 此复杂类型是抽象类。</span><span class="sxs-lookup"><span data-stu-id="169e4-109">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="169e4-110">引用的特定类型的列出的连接设置。</span><span class="sxs-lookup"><span data-stu-id="169e4-110">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="169e4-111">派生的类型</span><span class="sxs-lookup"><span data-stu-id="169e4-111">Derived types</span></span>
| <span data-ttu-id="169e4-112">Type</span><span class="sxs-lookup"><span data-stu-id="169e4-112">Type</span></span> | <span data-ttu-id="169e4-113">说明</span><span class="sxs-lookup"><span data-stu-id="169e4-113">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="169e4-114">**educationSynchronizationOAuth1ConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="169e4-114">**educationSynchronizationOAuth1ConnectionSettings**</span></span>](educationsynchronizationoauth1connectionsettings.md) | <span data-ttu-id="169e4-115">使用此类型提供 OAuth1 连接设置。</span><span class="sxs-lookup"><span data-stu-id="169e4-115">Use this type to provide OAuth1 connection settings.</span></span> |
| [<span data-ttu-id="169e4-116">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="169e4-116">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="169e4-117">使用此类型提供 OAuth2 客户端凭据授予连接设置。</span><span class="sxs-lookup"><span data-stu-id="169e4-117">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="169e4-118">属性</span><span class="sxs-lookup"><span data-stu-id="169e4-118">Properties</span></span>

| <span data-ttu-id="169e4-119">属性</span><span class="sxs-lookup"><span data-stu-id="169e4-119">Property</span></span> | <span data-ttu-id="169e4-120">类型</span><span class="sxs-lookup"><span data-stu-id="169e4-120">Type</span></span> | <span data-ttu-id="169e4-121">说明</span><span class="sxs-lookup"><span data-stu-id="169e4-121">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="169e4-122">**clientId**</span><span class="sxs-lookup"><span data-stu-id="169e4-122">**clientId**</span></span> | <span data-ttu-id="169e4-123">字符串</span><span class="sxs-lookup"><span data-stu-id="169e4-123">String</span></span> |  <span data-ttu-id="169e4-124">用于连接到提供程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="169e4-124">Client ID used to connect to the provider.</span></span> |
| <span data-ttu-id="169e4-125">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="169e4-125">**clientSecret**</span></span> | <span data-ttu-id="169e4-126">字符串</span><span class="sxs-lookup"><span data-stu-id="169e4-126">String</span></span> |  <span data-ttu-id="169e4-127">验证连接到提供程序的客户端机密。</span><span class="sxs-lookup"><span data-stu-id="169e4-127">Client secret to authenticate the connection to the provider.</span></span> |