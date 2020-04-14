---
title: emailCertificateType 枚举类型
description: 支持的电子邮件签名和加密的证书来源。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d2f5e4add7f67c6b772aa903d4e3b860b67ecbf5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460099"
---
# <a name="emailcertificatetype-enum-type"></a><span data-ttu-id="b2ad5-103">emailCertificateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b2ad5-103">emailCertificateType enum type</span></span>

<span data-ttu-id="b2ad5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2ad5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2ad5-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b2ad5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2ad5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b2ad5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2ad5-107">支持的电子邮件签名和加密的证书来源。</span><span class="sxs-lookup"><span data-stu-id="b2ad5-107">Supported certificate sources for email signing and encryption.</span></span>

## <a name="members"></a><span data-ttu-id="b2ad5-108">成员</span><span class="sxs-lookup"><span data-stu-id="b2ad5-108">Members</span></span>
|<span data-ttu-id="b2ad5-109">成员</span><span class="sxs-lookup"><span data-stu-id="b2ad5-109">Member</span></span>|<span data-ttu-id="b2ad5-110">值</span><span class="sxs-lookup"><span data-stu-id="b2ad5-110">Value</span></span>|<span data-ttu-id="b2ad5-111">说明</span><span class="sxs-lookup"><span data-stu-id="b2ad5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2ad5-112">无</span><span class="sxs-lookup"><span data-stu-id="b2ad5-112">none</span></span>|<span data-ttu-id="b2ad5-113">0</span><span class="sxs-lookup"><span data-stu-id="b2ad5-113">0</span></span>|<span data-ttu-id="b2ad5-114">不要将证书用作源。</span><span class="sxs-lookup"><span data-stu-id="b2ad5-114">Do not use a certificate as a source.</span></span>|
|<span data-ttu-id="b2ad5-115">证书</span><span class="sxs-lookup"><span data-stu-id="b2ad5-115">certificate</span></span>|<span data-ttu-id="b2ad5-116">1</span><span class="sxs-lookup"><span data-stu-id="b2ad5-116">1</span></span>|<span data-ttu-id="b2ad5-117">对证书源使用证书。</span><span class="sxs-lookup"><span data-stu-id="b2ad5-117">Use an certificate for certificate source.</span></span>|
|<span data-ttu-id="b2ad5-118">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="b2ad5-118">derivedCredential</span></span>|<span data-ttu-id="b2ad5-119">双面</span><span class="sxs-lookup"><span data-stu-id="b2ad5-119">2</span></span>|<span data-ttu-id="b2ad5-120">对证书源使用派生凭据。</span><span class="sxs-lookup"><span data-stu-id="b2ad5-120">Use a derived credential for certificate source.</span></span>|



