---
title: firewallCertificateRevocationListCheckMethodType 枚举类型
description: FirewallCertificateRevocationListCheckMethod 的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 832df7bfacbbba9643f4e1181f454bc60038ffb0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36338152"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="84e33-103">firewallCertificateRevocationListCheckMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="84e33-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="84e33-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="84e33-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84e33-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="84e33-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84e33-106">FirewallCertificateRevocationListCheckMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="84e33-106">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="84e33-107">成员</span><span class="sxs-lookup"><span data-stu-id="84e33-107">Members</span></span>
|<span data-ttu-id="84e33-108">成员</span><span class="sxs-lookup"><span data-stu-id="84e33-108">Member</span></span>|<span data-ttu-id="84e33-109">值</span><span class="sxs-lookup"><span data-stu-id="84e33-109">Value</span></span>|<span data-ttu-id="84e33-110">说明</span><span class="sxs-lookup"><span data-stu-id="84e33-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84e33-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="84e33-111">deviceDefault</span></span>|<span data-ttu-id="84e33-112">0</span><span class="sxs-lookup"><span data-stu-id="84e33-112">0</span></span>|<span data-ttu-id="84e33-113">没有由 Intune 配置的值, 请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="84e33-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="84e33-114">无</span><span class="sxs-lookup"><span data-stu-id="84e33-114">none</span></span>|<span data-ttu-id="84e33-115">1</span><span class="sxs-lookup"><span data-stu-id="84e33-115">1</span></span>|<span data-ttu-id="84e33-116">不检查证书吊销列表</span><span class="sxs-lookup"><span data-stu-id="84e33-116">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="84e33-117">应试</span><span class="sxs-lookup"><span data-stu-id="84e33-117">attempt</span></span>|<span data-ttu-id="84e33-118">双面</span><span class="sxs-lookup"><span data-stu-id="84e33-118">2</span></span>|<span data-ttu-id="84e33-119">仅当支票确认证书时, 才尝试 CRL 检查并允许证书</span><span class="sxs-lookup"><span data-stu-id="84e33-119">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="84e33-120">无须</span><span class="sxs-lookup"><span data-stu-id="84e33-120">require</span></span>|<span data-ttu-id="84e33-121">第三章</span><span class="sxs-lookup"><span data-stu-id="84e33-121">3</span></span>|<span data-ttu-id="84e33-122">在允许证书之前, 需要进行成功的 CRL 检查</span><span class="sxs-lookup"><span data-stu-id="84e33-122">Require a successful CRL check before allowing a certificate</span></span>|



