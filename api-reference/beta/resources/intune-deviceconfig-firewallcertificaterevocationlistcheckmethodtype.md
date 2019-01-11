---
title: firewallCertificateRevocationListCheckMethodType 枚举类型
description: FirewallCertificateRevocationListCheckMethod 的可能值
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c300b1d3c73cc4ae19ef1282c00d00800243b4b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889276"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="05f8d-103">firewallCertificateRevocationListCheckMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="05f8d-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="05f8d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="05f8d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05f8d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="05f8d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="05f8d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="05f8d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05f8d-107">FirewallCertificateRevocationListCheckMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="05f8d-107">Possible values for firewallCertificateRevocationListCheckMethod</span></span>
## <a name="members"></a><span data-ttu-id="05f8d-108">成员</span><span class="sxs-lookup"><span data-stu-id="05f8d-108">Members</span></span>
|<span data-ttu-id="05f8d-109">成员</span><span class="sxs-lookup"><span data-stu-id="05f8d-109">Member</span></span>|<span data-ttu-id="05f8d-110">值</span><span class="sxs-lookup"><span data-stu-id="05f8d-110">Value</span></span>|<span data-ttu-id="05f8d-111">Description</span><span class="sxs-lookup"><span data-stu-id="05f8d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05f8d-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="05f8d-112">deviceDefault</span></span>|<span data-ttu-id="05f8d-113">0</span><span class="sxs-lookup"><span data-stu-id="05f8d-113">0</span></span>|<span data-ttu-id="05f8d-114">配置通过 Intune，没有值不会替代的用户配置设备默认值</span><span class="sxs-lookup"><span data-stu-id="05f8d-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="05f8d-115">无</span><span class="sxs-lookup"><span data-stu-id="05f8d-115">none</span></span>|<span data-ttu-id="05f8d-116">1</span><span class="sxs-lookup"><span data-stu-id="05f8d-116">1</span></span>|<span data-ttu-id="05f8d-117">不检查证书吊销列表</span><span class="sxs-lookup"><span data-stu-id="05f8d-117">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="05f8d-118">尝试</span><span class="sxs-lookup"><span data-stu-id="05f8d-118">attempt</span></span>|<span data-ttu-id="05f8d-119">2</span><span class="sxs-lookup"><span data-stu-id="05f8d-119">2</span></span>|<span data-ttu-id="05f8d-120">尝试 CRL 检查并检查确认证书时才允许证书</span><span class="sxs-lookup"><span data-stu-id="05f8d-120">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="05f8d-121">需要</span><span class="sxs-lookup"><span data-stu-id="05f8d-121">require</span></span>|<span data-ttu-id="05f8d-122">3</span><span class="sxs-lookup"><span data-stu-id="05f8d-122">3</span></span>|<span data-ttu-id="05f8d-123">需要之前允许证书的 CRL 检查成功</span><span class="sxs-lookup"><span data-stu-id="05f8d-123">Require a successful CRL check before allowing a certificate</span></span>|





