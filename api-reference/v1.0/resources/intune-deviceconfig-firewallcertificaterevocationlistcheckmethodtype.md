---
title: firewallCertificateRevocationListCheckMethodType 枚举类型
description: FirewallCertificateRevocationListCheckMethod 的可能值
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2beee8f7c4f049aa1918b7e1516c3ce586a8cad0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839947"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="2fd54-103">firewallCertificateRevocationListCheckMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2fd54-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="2fd54-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2fd54-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2fd54-105">FirewallCertificateRevocationListCheckMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="2fd54-105">Possible values for firewallCertificateRevocationListCheckMethod</span></span>
## <a name="members"></a><span data-ttu-id="2fd54-106">成员</span><span class="sxs-lookup"><span data-stu-id="2fd54-106">Members</span></span>
|<span data-ttu-id="2fd54-107">成员</span><span class="sxs-lookup"><span data-stu-id="2fd54-107">Member</span></span>|<span data-ttu-id="2fd54-108">值</span><span class="sxs-lookup"><span data-stu-id="2fd54-108">Value</span></span>|<span data-ttu-id="2fd54-109">Description</span><span class="sxs-lookup"><span data-stu-id="2fd54-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fd54-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="2fd54-110">deviceDefault</span></span>|<span data-ttu-id="2fd54-111">0</span><span class="sxs-lookup"><span data-stu-id="2fd54-111">0</span></span>|<span data-ttu-id="2fd54-112">配置通过 Intune，没有值不会替代的用户配置设备默认值</span><span class="sxs-lookup"><span data-stu-id="2fd54-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="2fd54-113">无</span><span class="sxs-lookup"><span data-stu-id="2fd54-113">none</span></span>|<span data-ttu-id="2fd54-114">1</span><span class="sxs-lookup"><span data-stu-id="2fd54-114">1</span></span>|<span data-ttu-id="2fd54-115">不检查证书吊销列表</span><span class="sxs-lookup"><span data-stu-id="2fd54-115">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="2fd54-116">尝试</span><span class="sxs-lookup"><span data-stu-id="2fd54-116">attempt</span></span>|<span data-ttu-id="2fd54-117">2</span><span class="sxs-lookup"><span data-stu-id="2fd54-117">2</span></span>|<span data-ttu-id="2fd54-118">尝试 CRL 检查并检查确认证书时才允许证书</span><span class="sxs-lookup"><span data-stu-id="2fd54-118">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="2fd54-119">需要</span><span class="sxs-lookup"><span data-stu-id="2fd54-119">require</span></span>|<span data-ttu-id="2fd54-120">3</span><span class="sxs-lookup"><span data-stu-id="2fd54-120">3</span></span>|<span data-ttu-id="2fd54-121">需要之前允许证书的 CRL 检查成功</span><span class="sxs-lookup"><span data-stu-id="2fd54-121">Require a successful CRL check before allowing a certificate</span></span>|



