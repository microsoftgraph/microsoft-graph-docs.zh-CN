---
title: firewallCertificateRevocationListCheckMethodType 枚举类型
description: FirewallCertificateRevocationListCheckMethod 的可能值
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4585c30c0a910befd8df8482636916af9ad9c0d6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396411"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="d22ec-103">firewallCertificateRevocationListCheckMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d22ec-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="d22ec-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="d22ec-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d22ec-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d22ec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d22ec-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d22ec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d22ec-107">FirewallCertificateRevocationListCheckMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="d22ec-107">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="d22ec-108">成员</span><span class="sxs-lookup"><span data-stu-id="d22ec-108">Members</span></span>
|<span data-ttu-id="d22ec-109">成员</span><span class="sxs-lookup"><span data-stu-id="d22ec-109">Member</span></span>|<span data-ttu-id="d22ec-110">值</span><span class="sxs-lookup"><span data-stu-id="d22ec-110">Value</span></span>|<span data-ttu-id="d22ec-111">说明</span><span class="sxs-lookup"><span data-stu-id="d22ec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d22ec-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="d22ec-112">deviceDefault</span></span>|<span data-ttu-id="d22ec-113">0</span><span class="sxs-lookup"><span data-stu-id="d22ec-113">0</span></span>|<span data-ttu-id="d22ec-114">配置通过 Intune，没有值不会替代的用户配置设备默认值</span><span class="sxs-lookup"><span data-stu-id="d22ec-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="d22ec-115">无</span><span class="sxs-lookup"><span data-stu-id="d22ec-115">none</span></span>|<span data-ttu-id="d22ec-116">1</span><span class="sxs-lookup"><span data-stu-id="d22ec-116">1</span></span>|<span data-ttu-id="d22ec-117">不检查证书吊销列表</span><span class="sxs-lookup"><span data-stu-id="d22ec-117">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="d22ec-118">尝试</span><span class="sxs-lookup"><span data-stu-id="d22ec-118">attempt</span></span>|<span data-ttu-id="d22ec-119">2</span><span class="sxs-lookup"><span data-stu-id="d22ec-119">2</span></span>|<span data-ttu-id="d22ec-120">尝试 CRL 检查并检查确认证书时才允许证书</span><span class="sxs-lookup"><span data-stu-id="d22ec-120">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="d22ec-121">需要</span><span class="sxs-lookup"><span data-stu-id="d22ec-121">require</span></span>|<span data-ttu-id="d22ec-122">3</span><span class="sxs-lookup"><span data-stu-id="d22ec-122">3</span></span>|<span data-ttu-id="d22ec-123">需要之前允许证书的 CRL 检查成功</span><span class="sxs-lookup"><span data-stu-id="d22ec-123">Require a successful CRL check before allowing a certificate</span></span>|




