---
title: educationSynchronizationConnectionSettings 资源类型
description: '表示提供程序连接设置。 这使系统可以了解如何连接到提供程序 api。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 387c002240d54d1ec12e58564e91831d6f0e8a50
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334104"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="b3399-104">educationSynchronizationConnectionSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="b3399-104">educationSynchronizationConnectionSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3399-105">表示提供程序连接设置。</span><span class="sxs-lookup"><span data-stu-id="b3399-105">Represents the provider connection settings.</span></span> <span data-ttu-id="b3399-106">这使系统可以了解如何连接到提供程序 api。</span><span class="sxs-lookup"><span data-stu-id="b3399-106">This allows the system to know how to connect to the provider APIs.</span></span> 

> <span data-ttu-id="b3399-107">**注意:** 此复杂类型是抽象的。</span><span class="sxs-lookup"><span data-stu-id="b3399-107">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="b3399-108">请参阅列出的特定类型的连接设置。</span><span class="sxs-lookup"><span data-stu-id="b3399-108">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="b3399-109">派生类型</span><span class="sxs-lookup"><span data-stu-id="b3399-109">Derived types</span></span>
| <span data-ttu-id="b3399-110">类型</span><span class="sxs-lookup"><span data-stu-id="b3399-110">Type</span></span> | <span data-ttu-id="b3399-111">说明</span><span class="sxs-lookup"><span data-stu-id="b3399-111">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="b3399-112">**educationSynchronizationOAuth1ConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="b3399-112">**educationSynchronizationOAuth1ConnectionSettings**</span></span>](educationsynchronizationoauth1connectionsettings.md) | <span data-ttu-id="b3399-113">使用此类型可提供 OAuth1 连接设置。</span><span class="sxs-lookup"><span data-stu-id="b3399-113">Use this type to provide OAuth1 connection settings.</span></span> |
| [<span data-ttu-id="b3399-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="b3399-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="b3399-115">使用此类型可提供 OAuth2 客户端凭据授予连接设置。</span><span class="sxs-lookup"><span data-stu-id="b3399-115">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="b3399-116">属性</span><span class="sxs-lookup"><span data-stu-id="b3399-116">Properties</span></span>

| <span data-ttu-id="b3399-117">属性</span><span class="sxs-lookup"><span data-stu-id="b3399-117">Property</span></span> | <span data-ttu-id="b3399-118">类型</span><span class="sxs-lookup"><span data-stu-id="b3399-118">Type</span></span> | <span data-ttu-id="b3399-119">说明</span><span class="sxs-lookup"><span data-stu-id="b3399-119">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="b3399-120">**clientId**</span><span class="sxs-lookup"><span data-stu-id="b3399-120">**clientId**</span></span> | <span data-ttu-id="b3399-121">String</span><span class="sxs-lookup"><span data-stu-id="b3399-121">String</span></span> |  <span data-ttu-id="b3399-122">用于连接到提供程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="b3399-122">Client ID used to connect to the provider.</span></span> |
| <span data-ttu-id="b3399-123">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="b3399-123">**clientSecret**</span></span> | <span data-ttu-id="b3399-124">String</span><span class="sxs-lookup"><span data-stu-id="b3399-124">String</span></span> |  <span data-ttu-id="b3399-125">用于对与提供程序的连接进行身份验证的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="b3399-125">Client secret to authenticate the connection to the provider.</span></span> |
