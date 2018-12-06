---
title: Microsoft Graph 安全性 API 数据流
description: Microsoft Graph 安全性 API 在 Microsoft Graph 安全性生态系统中联合了对所有提供商的请求。 这基于应用程序提供的安全性提供商许可，如下图所示。 此许可工作流仅适用于非 Microsoft 提供商。
ms.openlocfilehash: 1e8b074e3cf4589ca67364ed7e225a62f40300fd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091845"
---
# <a name="microsoft-graph-security-api-data-flow"></a><span data-ttu-id="b4798-105">Microsoft Graph 安全性 API 数据流</span><span class="sxs-lookup"><span data-stu-id="b4798-105">Microsoft Graph Security API data flow</span></span>

<span data-ttu-id="b4798-106">Microsoft Graph 安全性 API 在 Microsoft Graph 安全性生态系统中联合了对所有提供商的请求。</span><span class="sxs-lookup"><span data-stu-id="b4798-106">The Microsoft Graph Security API federates requests to all providers in the Microsoft Graph Security ecosystem.</span></span> <span data-ttu-id="b4798-107">这基于应用程序提供的安全性提供商许可，如下图所示。</span><span class="sxs-lookup"><span data-stu-id="b4798-107">This is based on the security provider consent provided by the application, as shown in the following diagram.</span></span> <span data-ttu-id="b4798-108">此许可工作流仅适用于非 Microsoft 提供商。</span><span class="sxs-lookup"><span data-stu-id="b4798-108">The consent workflow only applies to non-Microsoft providers.</span></span>

![security_dataflow_1.png](./images/security-dataflow-1.png)

<span data-ttu-id="b4798-110">以下是对此流的说明：</span><span class="sxs-lookup"><span data-stu-id="b4798-110">The following is a description of the flow:</span></span>

1. <span data-ttu-id="b4798-111">应用程序用户登录到提供商应用程序，以查看提供商提供的许可表单。</span><span class="sxs-lookup"><span data-stu-id="b4798-111">The application user signs in to the provider application to view the consent form from the provider.</span></span> <span data-ttu-id="b4798-112">此许可表单体验或 UI 的所有权属于提供商，且仅适用于非 Microsoft 提供商用于获取其客户对向 Microsoft Graph 安全性 API 发送请求的明确许可。</span><span class="sxs-lookup"><span data-stu-id="b4798-112">This consent form experience or UI is owned by the provider and applies to non-Microsoft providers only to get explicit consent from their customers to send requests to Microsoft Graph Security API.</span></span>
2. <span data-ttu-id="b4798-113">客户端许可存储在提供商端。</span><span class="sxs-lookup"><span data-stu-id="b4798-113">The client consent is stored on the provider side.</span></span>
3. <span data-ttu-id="b4798-114">提供商许可服务调用 Microsoft Graph 安全性 API，来告知相应客户的许可批准。</span><span class="sxs-lookup"><span data-stu-id="b4798-114">The provider consent service calls the Microsoft Graph Security API to inform consent approval for the respective customer.</span></span>
4. <span data-ttu-id="b4798-115">应用程序向 Microsoft Graph 安全性 API 发送请求。</span><span class="sxs-lookup"><span data-stu-id="b4798-115">The application sends a request to the Microsoft Graph Security API.</span></span>
5. <span data-ttu-id="b4798-116">Microsoft Graph 安全性 API 查看此客户映射到各个提供商的许可信息。</span><span class="sxs-lookup"><span data-stu-id="b4798-116">The Microsoft Graph Security API checks for the consent information for this customer mapped to various providers.</span></span>
6. <span data-ttu-id="b4798-117">Microsoft Graph 安全性 API 调用此客户已通过提供商许可体验明确许可的所有提供商。</span><span class="sxs-lookup"><span data-stu-id="b4798-117">The Microsoft Graph Security API calls all those providers the customer has given explicit consent to via the provider consent experience.</span></span>
7. <span data-ttu-id="b4798-118">从该客户端的所有已许可的提供商返回响应。</span><span class="sxs-lookup"><span data-stu-id="b4798-118">The response is returned from all the consented providers for that client.</span></span>
8. <span data-ttu-id="b4798-119">结果集响应返回至应用程序。</span><span class="sxs-lookup"><span data-stu-id="b4798-119">The result set response is returned to the application.</span></span>
9. <span data-ttu-id="b4798-120">若客户尚未许可任何提供商，则响应不包括任何提供商提供的结果。</span><span class="sxs-lookup"><span data-stu-id="b4798-120">If the customer has not consented to any provider, no results from those providers are included in the response.</span></span>
