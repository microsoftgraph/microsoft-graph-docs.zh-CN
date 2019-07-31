---
title: educationSynchronizationConnectionSettings 资源类型
description: '表示提供程序连接设置。 这使系统可以了解如何连接到提供程序 Api。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c82d912b13ca68dcdccd5ace0232ed65f92cd879
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972484"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="b4868-104">educationSynchronizationConnectionSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="b4868-104">educationSynchronizationConnectionSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4868-105">表示提供程序连接设置。</span><span class="sxs-lookup"><span data-stu-id="b4868-105">Represents the provider connection settings.</span></span> <span data-ttu-id="b4868-106">这使系统可以了解如何连接到提供程序 Api。</span><span class="sxs-lookup"><span data-stu-id="b4868-106">This allows the system to know how to connect to the provider APIs.</span></span> 

> <span data-ttu-id="b4868-107">**注意:** 此复杂类型是抽象的。</span><span class="sxs-lookup"><span data-stu-id="b4868-107">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="b4868-108">请参阅列出的特定类型的连接设置。</span><span class="sxs-lookup"><span data-stu-id="b4868-108">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="b4868-109">派生类型</span><span class="sxs-lookup"><span data-stu-id="b4868-109">Derived types</span></span>
| <span data-ttu-id="b4868-110">类型</span><span class="sxs-lookup"><span data-stu-id="b4868-110">Type</span></span> | <span data-ttu-id="b4868-111">说明</span><span class="sxs-lookup"><span data-stu-id="b4868-111">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="b4868-112">**educationSynchronizationOAuth1ConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="b4868-112">**educationSynchronizationOAuth1ConnectionSettings**</span></span>](educationsynchronizationoauth1connectionsettings.md) | <span data-ttu-id="b4868-113">使用此类型可提供 OAuth1 连接设置。</span><span class="sxs-lookup"><span data-stu-id="b4868-113">Use this type to provide OAuth1 connection settings.</span></span> |
| [<span data-ttu-id="b4868-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="b4868-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="b4868-115">使用此类型可提供 OAuth2 客户端凭据授予连接设置。</span><span class="sxs-lookup"><span data-stu-id="b4868-115">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="b4868-116">属性</span><span class="sxs-lookup"><span data-stu-id="b4868-116">Properties</span></span>

| <span data-ttu-id="b4868-117">属性</span><span class="sxs-lookup"><span data-stu-id="b4868-117">Property</span></span> | <span data-ttu-id="b4868-118">类型</span><span class="sxs-lookup"><span data-stu-id="b4868-118">Type</span></span> | <span data-ttu-id="b4868-119">说明</span><span class="sxs-lookup"><span data-stu-id="b4868-119">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="b4868-120">**clientId**</span><span class="sxs-lookup"><span data-stu-id="b4868-120">**clientId**</span></span> | <span data-ttu-id="b4868-121">String</span><span class="sxs-lookup"><span data-stu-id="b4868-121">String</span></span> |  <span data-ttu-id="b4868-122">用于连接到提供程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="b4868-122">Client ID used to connect to the provider.</span></span> |
| <span data-ttu-id="b4868-123">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="b4868-123">**clientSecret**</span></span> | <span data-ttu-id="b4868-124">String</span><span class="sxs-lookup"><span data-stu-id="b4868-124">String</span></span> |  <span data-ttu-id="b4868-125">用于对与提供程序的连接进行身份验证的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="b4868-125">Client secret to authenticate the connection to the provider.</span></span> |
