---
title: emailCertificateType 枚举类型
description: 支持的电子邮件签名和加密的证书来源。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 691923c70c89d2f29cb45f6f3a994bbc919a7d56
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48705972"
---
# <a name="emailcertificatetype-enum-type"></a><span data-ttu-id="7341a-103">emailCertificateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7341a-103">emailCertificateType enum type</span></span>

<span data-ttu-id="7341a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7341a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7341a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7341a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7341a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7341a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7341a-107">支持的电子邮件签名和加密的证书来源。</span><span class="sxs-lookup"><span data-stu-id="7341a-107">Supported certificate sources for email signing and encryption.</span></span>

## <a name="members"></a><span data-ttu-id="7341a-108">成员</span><span class="sxs-lookup"><span data-stu-id="7341a-108">Members</span></span>
|<span data-ttu-id="7341a-109">成员</span><span class="sxs-lookup"><span data-stu-id="7341a-109">Member</span></span>|<span data-ttu-id="7341a-110">值</span><span class="sxs-lookup"><span data-stu-id="7341a-110">Value</span></span>|<span data-ttu-id="7341a-111">说明</span><span class="sxs-lookup"><span data-stu-id="7341a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7341a-112">无</span><span class="sxs-lookup"><span data-stu-id="7341a-112">none</span></span>|<span data-ttu-id="7341a-113">0</span><span class="sxs-lookup"><span data-stu-id="7341a-113">0</span></span>|<span data-ttu-id="7341a-114">不要将证书用作源。</span><span class="sxs-lookup"><span data-stu-id="7341a-114">Do not use a certificate as a source.</span></span>|
|<span data-ttu-id="7341a-115">证书</span><span class="sxs-lookup"><span data-stu-id="7341a-115">certificate</span></span>|<span data-ttu-id="7341a-116">1</span><span class="sxs-lookup"><span data-stu-id="7341a-116">1</span></span>|<span data-ttu-id="7341a-117">对证书源使用证书。</span><span class="sxs-lookup"><span data-stu-id="7341a-117">Use an certificate for certificate source.</span></span>|
|<span data-ttu-id="7341a-118">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="7341a-118">derivedCredential</span></span>|<span data-ttu-id="7341a-119">双面</span><span class="sxs-lookup"><span data-stu-id="7341a-119">2</span></span>|<span data-ttu-id="7341a-120">对证书源使用派生凭据。</span><span class="sxs-lookup"><span data-stu-id="7341a-120">Use a derived credential for certificate source.</span></span>|





