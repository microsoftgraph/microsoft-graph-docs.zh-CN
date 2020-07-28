---
title: educationSynchronizationConnectionSettings 资源类型
description: '表示提供程序连接设置。 这使系统可以了解如何连接到提供程序 Api。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 71da1acbd9910757375acbc22dda63f412f459b2
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434877"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="d2dfe-104">educationSynchronizationConnectionSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="d2dfe-104">educationSynchronizationConnectionSettings resource type</span></span>

<span data-ttu-id="d2dfe-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2dfe-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2dfe-106">表示提供程序连接设置。</span><span class="sxs-lookup"><span data-stu-id="d2dfe-106">Represents the provider connection settings.</span></span> <span data-ttu-id="d2dfe-107">这使系统可以了解如何连接到提供程序 Api。</span><span class="sxs-lookup"><span data-stu-id="d2dfe-107">This allows the system to know how to connect to the provider APIs.</span></span>

> [!NOTE]
> <span data-ttu-id="d2dfe-108">此复杂类型是抽象的。</span><span class="sxs-lookup"><span data-stu-id="d2dfe-108">This complex type is abstract.</span></span> <span data-ttu-id="d2dfe-109">请参阅列出的特定类型的连接设置。</span><span class="sxs-lookup"><span data-stu-id="d2dfe-109">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="d2dfe-110">派生类型</span><span class="sxs-lookup"><span data-stu-id="d2dfe-110">Derived types</span></span>

| <span data-ttu-id="d2dfe-111">类型</span><span class="sxs-lookup"><span data-stu-id="d2dfe-111">Type</span></span>                                                                                                                                      | <span data-ttu-id="d2dfe-112">说明</span><span class="sxs-lookup"><span data-stu-id="d2dfe-112">Description</span></span>                                                                   |
| :---------------------------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------- |
| [<span data-ttu-id="d2dfe-113">educationSynchronizationOAuth1ConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="d2dfe-113">educationSynchronizationOAuth1ConnectionSettings</span></span>](educationsynchronizationoauth1connectionsettings.md)                                   | <span data-ttu-id="d2dfe-114">使用此类型可提供 OAuth1 连接设置。</span><span class="sxs-lookup"><span data-stu-id="d2dfe-114">Use this type to provide OAuth1 connection settings.</span></span>                          |
| [<span data-ttu-id="d2dfe-115">educationSynchronizationOAuth2ClientCredentialsConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="d2dfe-115">educationSynchronizationOAuth2ClientCredentialsConnectionSettings</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="d2dfe-116">使用此类型可提供 OAuth2 客户端凭据授予连接设置。</span><span class="sxs-lookup"><span data-stu-id="d2dfe-116">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="d2dfe-117">属性</span><span class="sxs-lookup"><span data-stu-id="d2dfe-117">Properties</span></span>

| <span data-ttu-id="d2dfe-118">属性</span><span class="sxs-lookup"><span data-stu-id="d2dfe-118">Property</span></span>     | <span data-ttu-id="d2dfe-119">类型</span><span class="sxs-lookup"><span data-stu-id="d2dfe-119">Type</span></span>   | <span data-ttu-id="d2dfe-120">说明</span><span class="sxs-lookup"><span data-stu-id="d2dfe-120">Description</span></span>                                                   |
| :----------- | :----- | :------------------------------------------------------------ |
| <span data-ttu-id="d2dfe-121">clientId</span><span class="sxs-lookup"><span data-stu-id="d2dfe-121">clientId</span></span>     | <span data-ttu-id="d2dfe-122">字符串</span><span class="sxs-lookup"><span data-stu-id="d2dfe-122">String</span></span> | <span data-ttu-id="d2dfe-123">用于连接到提供程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="d2dfe-123">Client ID used to connect to the provider.</span></span>                    |
| <span data-ttu-id="d2dfe-124">clientSecret</span><span class="sxs-lookup"><span data-stu-id="d2dfe-124">clientSecret</span></span> | <span data-ttu-id="d2dfe-125">字符串</span><span class="sxs-lookup"><span data-stu-id="d2dfe-125">String</span></span> | <span data-ttu-id="d2dfe-126">用于对与提供程序的连接进行身份验证的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="d2dfe-126">Client secret to authenticate the connection to the provider.</span></span> |
