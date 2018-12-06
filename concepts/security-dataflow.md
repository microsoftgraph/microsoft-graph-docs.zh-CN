---
title: Microsoft Graph 安全 API 数据流
description: Microsoft Graph 安全 API 建立联盟与 Microsoft Graph Security 生态系统中的所有提供商的请求。 这基于应用程序，提供安全提供程序同意，如下图中所示。 同意工作流仅适用于非 Microsoft 提供程序。
ms.openlocfilehash: 1e8b074e3cf4589ca67364ed7e225a62f40300fd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091845"
---
# <a name="microsoft-graph-security-api-data-flow"></a><span data-ttu-id="4b2d5-105">Microsoft Graph 安全 API 数据流</span><span class="sxs-lookup"><span data-stu-id="4b2d5-105">Microsoft Graph Security API data flow</span></span>

<span data-ttu-id="4b2d5-106">Microsoft Graph 安全 API 建立联盟与 Microsoft Graph Security 生态系统中的所有提供商的请求。</span><span class="sxs-lookup"><span data-stu-id="4b2d5-106">The Microsoft Graph Security API federates requests to all providers in the Microsoft Graph Security ecosystem.</span></span> <span data-ttu-id="4b2d5-107">这基于应用程序，提供安全提供程序同意，如下图中所示。</span><span class="sxs-lookup"><span data-stu-id="4b2d5-107">This is based on the security provider consent provided by the application, as shown in the following diagram.</span></span> <span data-ttu-id="4b2d5-108">同意工作流仅适用于非 Microsoft 提供程序。</span><span class="sxs-lookup"><span data-stu-id="4b2d5-108">The consent workflow only applies to non-Microsoft providers.</span></span>

![security_dataflow_1.png](./images/security-dataflow-1.png)

<span data-ttu-id="4b2d5-110">以下是流的说明：</span><span class="sxs-lookup"><span data-stu-id="4b2d5-110">The following is a description of the flow:</span></span>

1. <span data-ttu-id="4b2d5-111">应用程序用户登录到要查看从提供程序的同意窗体的提供程序应用程序。</span><span class="sxs-lookup"><span data-stu-id="4b2d5-111">The application user signs in to the provider application to view the consent form from the provider.</span></span> <span data-ttu-id="4b2d5-112">此窗体的同意体验或 UI 由提供程序，适用于非 Microsoft 提供程序仅要从其客户将请求发送到 Microsoft Graph 安全 API 获取明确同意。</span><span class="sxs-lookup"><span data-stu-id="4b2d5-112">This consent form experience or UI is owned by the provider and applies to non-Microsoft providers only to get explicit consent from their customers to send requests to Microsoft Graph Security API.</span></span>
2. <span data-ttu-id="4b2d5-113">客户端同意存储提供程序侧。</span><span class="sxs-lookup"><span data-stu-id="4b2d5-113">The client consent is stored on the provider side.</span></span>
3. <span data-ttu-id="4b2d5-114">提供程序 consent 服务调用 Microsoft Graph 安全 API，告知各自的客户的同意审批。</span><span class="sxs-lookup"><span data-stu-id="4b2d5-114">The provider consent service calls the Microsoft Graph Security API to inform consent approval for the respective customer.</span></span>
4. <span data-ttu-id="4b2d5-115">应用程序将请求发送到 Microsoft Graph 安全 API。</span><span class="sxs-lookup"><span data-stu-id="4b2d5-115">The application sends a request to the Microsoft Graph Security API.</span></span>
5. <span data-ttu-id="4b2d5-116">Microsoft Graph 安全 API 检查此客户映射到不同的提供程序的许可信息。</span><span class="sxs-lookup"><span data-stu-id="4b2d5-116">The Microsoft Graph Security API checks for the consent information for this customer mapped to various providers.</span></span>
6. <span data-ttu-id="4b2d5-117">Microsoft Graph 安全 API 调用所有客户提供了通过提供程序同意体验的明确同意这些提供程序。</span><span class="sxs-lookup"><span data-stu-id="4b2d5-117">The Microsoft Graph Security API calls all those providers the customer has given explicit consent to via the provider consent experience.</span></span>
7. <span data-ttu-id="4b2d5-118">从该客户端的 consented 提供程序返回的响应。</span><span class="sxs-lookup"><span data-stu-id="4b2d5-118">The response is returned from all the consented providers for that client.</span></span>
8. <span data-ttu-id="4b2d5-119">结果集响应返回到应用程序。</span><span class="sxs-lookup"><span data-stu-id="4b2d5-119">The result set response is returned to the application.</span></span>
9. <span data-ttu-id="4b2d5-120">如果客户已不同意任何提供程序，在响应中不包含这些提供程序的任何结果。</span><span class="sxs-lookup"><span data-stu-id="4b2d5-120">If the customer has not consented to any provider, no results from those providers are included in the response.</span></span>
