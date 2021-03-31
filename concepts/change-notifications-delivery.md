---
title: 以不同方式接收更改通知
description: 更改通知可以通过不同的技术来传送，包括 Webhook 和 Azure 事件中心。
author: Jumaodhiss
localization_priority: Priority
ms.custom: graphiamtop20, devx-track-azurecli
ms.openlocfilehash: 2cb6000b309b9bcaf5af840cc26976c7254d2d96
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469099"
---
# <a name="get-change-notifications-delivered-in-different-ways-preview"></a><span data-ttu-id="367b2-103">获取通过不同方式传送的更改通知（预览版）</span><span class="sxs-lookup"><span data-stu-id="367b2-103">Get change notifications delivered in different ways (preview)</span></span>

<span data-ttu-id="367b2-104">可通过不同方式向订阅者传送更改通知。</span><span class="sxs-lookup"><span data-stu-id="367b2-104">Change notifications can be delivered in different ways to subscribers.</span></span> <span data-ttu-id="367b2-105">如果更改通知的主要传送模式是 Webhook，则对于高吞吐量场景或当接收方无法公开公用的通知 URL 时，利用 Webhooks 可能很困难。</span><span class="sxs-lookup"><span data-stu-id="367b2-105">If the main delivery mode for change notifications is through webhooks, it can be challenging to take advantage of webhooks for high throughput scenarios or when the receiver cannot expose a publicly available notification URL.</span></span>  

<span data-ttu-id="367b2-106">此更改通知传递模式可用于支持 Microsoft Graph 更改通知的所有资源。</span><span class="sxs-lookup"><span data-stu-id="367b2-106">This change notifications delivery mode is available for all resources that support Microsoft Graph change notifications.</span></span>

<span data-ttu-id="367b2-107">高吞吐量场景的恰当例子包括订阅大量资源的应用程序、订阅频繁变更的资源的应用程序以及跨大量组织订阅资源的多租户应用程序。</span><span class="sxs-lookup"><span data-stu-id="367b2-107">Good examples of high throughput scenarios include applications subscribing to a large set of resources, applications subscribing to resources that change with a high frequency, and multi-tenant applications that subscribe to resources accross a large set of organizations.</span></span>

## <a name="using-azure-event-hubs-to-receive-change-notifications"></a><span data-ttu-id="367b2-108">使用 Azure 事件中心接收更改通知</span><span class="sxs-lookup"><span data-stu-id="367b2-108">Using Azure Event Hubs to receive change notifications</span></span>

<span data-ttu-id="367b2-109">[Azure 事件中心](https://azure.microsoft.com/services/event-hubs)是专为大规模部署而构建的常用实时事件引入和分发服务。</span><span class="sxs-lookup"><span data-stu-id="367b2-109">[Azure Event Hubs](https://azure.microsoft.com/services/event-hubs) is a popular real-time events ingestion and distribution service built for scale.</span></span> <span data-ttu-id="367b2-110">你可以使用 Azure 事件中心而不是传统 Webhook 来接收更改通知。</span><span class="sxs-lookup"><span data-stu-id="367b2-110">You can use Azure Events Hubs instead of traditional webhooks to receive change notifications.</span></span> <span data-ttu-id="367b2-111">此功能目前处于预览阶段。</span><span class="sxs-lookup"><span data-stu-id="367b2-111">This feature is currently in preview.</span></span>  
<span data-ttu-id="367b2-112">使用 Azure 事件中心接收更改通知与 Webhook 在某些方面有所不同，包括：</span><span class="sxs-lookup"><span data-stu-id="367b2-112">Using Azure Event Hubs to receive change notifications differs from webhooks in a few ways, including:</span></span>

- <span data-ttu-id="367b2-113">不依赖公开显示的通知 URL。</span><span class="sxs-lookup"><span data-stu-id="367b2-113">You don't rely on publicly exposed notification URLs.</span></span> <span data-ttu-id="367b2-114">事件中心 SDK 会将通知转发到你的应用程序。</span><span class="sxs-lookup"><span data-stu-id="367b2-114">The Event Hubs SDK will relay the notifications to your application.</span></span>
- <span data-ttu-id="367b2-115">无需恢复[通知 URL 验证](webhooks.md#notification-endpoint-validation)。</span><span class="sxs-lookup"><span data-stu-id="367b2-115">You don't need to reply to the [notification URL validation](webhooks.md#notification-endpoint-validation).</span></span> <span data-ttu-id="367b2-116">可忽略收到的验证消息。</span><span class="sxs-lookup"><span data-stu-id="367b2-116">You can ignore the validation message that you receive.</span></span>
- <span data-ttu-id="367b2-117">需要预配 Azure 事件中心。</span><span class="sxs-lookup"><span data-stu-id="367b2-117">You'll need to provision an Azure Event Hub.</span></span>
- <span data-ttu-id="367b2-118">需要预配 Azure 密钥保管库。</span><span class="sxs-lookup"><span data-stu-id="367b2-118">You'll need to provision an Azure Key Vault.</span></span>

### <a name="set-up-the-azure-keyvault-and-azure-event-hubs"></a><span data-ttu-id="367b2-119">设置 Azure 密钥保管库和 Azure 事件中心</span><span class="sxs-lookup"><span data-stu-id="367b2-119">Set up the Azure KeyVault and Azure Event Hubs</span></span>

<span data-ttu-id="367b2-120">本节将指导你完成所需的 Azure 服务设置。</span><span class="sxs-lookup"><span data-stu-id="367b2-120">This section will walk you through the setup of required Azure services.</span></span>

#### <a name="option-1-using-the-azure-cli"></a><span data-ttu-id="367b2-121">选项 1：使用 Azure CLI</span><span class="sxs-lookup"><span data-stu-id="367b2-121">Option 1: Using the Azure CLI</span></span>

<span data-ttu-id="367b2-122">[Azure CLI](/cli/azure/what-is-azure-cli) 允许你在 Azure 中编写脚本并自动执行管理任务。</span><span class="sxs-lookup"><span data-stu-id="367b2-122">The [Azure CLI](/cli/azure/what-is-azure-cli) allows you to script and automate adminstrative tasks in Azure.</span></span> <span data-ttu-id="367b2-123">可以[在本地计算机上安装](/cli/azure/install-azure-cli) CLI 或直接从 [Azure Cloud Shell](/azure/cloud-shell/quickstart) 运行。</span><span class="sxs-lookup"><span data-stu-id="367b2-123">The CLI can be [installed on your local computer](/cli/azure/install-azure-cli) or run directly from the [Azure Cloud Shell](/azure/cloud-shell/quickstart).</span></span>

```azurecli
# --------------
# TODO: update the following values
#sets the name of the resource group
resourcegroup=rg-graphevents-dev
#sets the location of the resources
location='uk south'
#sets the name of the Azure Event Hubs namespace
evhamespacename=evh-graphevents-dev
#sets the name of the hub under the namespace
evhhubname=graphevents
#sets the name of the access policy to the hub
evhpolicyname=grapheventspolicy
#sets the name of the Azure KeyVault
keyvaultname=kv-graphevents
#sets the name of the secret in Azure KeyVault that will contain the connection string to the hub
keyvaultsecretname=grapheventsconnectionstring
# --------------
az group create --location $location --name $resourcegroup
az eventhubs namespace create --name $evhamespacename --resource-group $resourcegroup --sku Basic --location $location
az eventhubs eventhub create --name $evhhubname --namespace-name $evhamespacename --resource-group $resourcegroup --partition-count 2 --message-retention 1
az eventhubs eventhub authorization-rule create --name $evhpolicyname --eventhub-name $evhhubname --namespace-name $evhamespacename --resource-group $resourcegroup --rights Send
evhprimaryconnectionstring=`az eventhubs eventhub authorization-rule keys list --name $evhpolicyname --eventhub-name $evhhubname --namespace-name $evhamespacename --resource-group $resourcegroup --query "primaryConnectionString" --output tsv`
az keyvault create --name $keyvaultname --resource-group $resourcegroup --location $location --enable-soft-delete true --sku standard --retention-days 90
az keyvault secret set --name $keyvaultsecretname --value $evhprimaryconnectionstring --vault-name $keyvaultname --output none
graphspn=`az ad sp list --display-name 'Microsoft Graph Change Tracking' --query "[].appId" --output tsv`
az keyvault set-policy --name $keyvaultname --resource-group $resourcegroup --secret-permissions get --spn $graphspn --output none
keyvaulturi=`az keyvault show --name $keyvaultname --resource-group $resourcegroup --query "properties.vaultUri" --output tsv`
domainname=`az ad signed-in-user show --query 'userPrincipalName' | cut -d '@' -f 2 | sed 's/\"//'`
notificationUrl="EventHub:${keyvaulturi}secrets/${keyvaultsecretname}?tenantId=${domainname}"
echo "Notification Url:\n${notificationUrl}"
```

> <span data-ttu-id="367b2-124">**注意：** 此处提供的脚本与基于 Linux 的 命令行管理程序、Windows WSL 和 Azure Cloud Shell 兼容。</span><span class="sxs-lookup"><span data-stu-id="367b2-124">**Note:** The script provided here is compatible with Linux based shells, Windows WSL, and Azure Cloud Shell.</span></span> <span data-ttu-id="367b2-125">它要求在 Windows 命令行管理程序中运行某些更新。</span><span class="sxs-lookup"><span data-stu-id="367b2-125">It will require some updates to run in Windows shells.</span></span>

#### <a name="option-2-using-the-azure-portal"></a><span data-ttu-id="367b2-126">选项 2：使用 Azure 门户</span><span class="sxs-lookup"><span data-stu-id="367b2-126">Option 2: Using the Azure Portal</span></span>

##### <a name="configuring-the-azure-event-hub"></a><span data-ttu-id="367b2-127">配置 Azure 事件中心</span><span class="sxs-lookup"><span data-stu-id="367b2-127">Configuring the Azure Event Hub</span></span>

<span data-ttu-id="367b2-128">在本节中，你将：</span><span class="sxs-lookup"><span data-stu-id="367b2-128">In this section you will:</span></span>

- <span data-ttu-id="367b2-129">创建 Azure 事件中心命名空间。</span><span class="sxs-lookup"><span data-stu-id="367b2-129">Create an Azure Event Hub namespace.</span></span>
- <span data-ttu-id="367b2-130">将中心添加到将转发和传送通知的该命名空间。</span><span class="sxs-lookup"><span data-stu-id="367b2-130">Add a hub to that namespace that will relay and deliver notifications.</span></span>
- <span data-ttu-id="367b2-131">添加共享访问策略，它将允许你获取新创建的中心的连接字符串。</span><span class="sxs-lookup"><span data-stu-id="367b2-131">Add a shared access policy that will allow you to get a connection string to the newly created hub.</span></span>

<span data-ttu-id="367b2-132">步骤：</span><span class="sxs-lookup"><span data-stu-id="367b2-132">Steps:</span></span>

1. <span data-ttu-id="367b2-133">打开浏览器以访问 [Azure 门户](https://portal.azure.com)。</span><span class="sxs-lookup"><span data-stu-id="367b2-133">Open a browser to the [Azure Portal](https://portal.azure.com).</span></span>
1. <span data-ttu-id="367b2-134">选择“**创建资源**”。</span><span class="sxs-lookup"><span data-stu-id="367b2-134">Select **Create a resource**.</span></span>
1. <span data-ttu-id="367b2-135">在搜索栏中键入“**事件中心**”。</span><span class="sxs-lookup"><span data-stu-id="367b2-135">Type **Event Hubs** in the search bar.</span></span>
1. <span data-ttu-id="367b2-136">选择“**事件中心**”建议。</span><span class="sxs-lookup"><span data-stu-id="367b2-136">Select the **Event Hubs** suggestion.</span></span> <span data-ttu-id="367b2-137">此时将加载“创建事件中心”页面。</span><span class="sxs-lookup"><span data-stu-id="367b2-137">The Event Hubs creation page will load.</span></span>  
1. <span data-ttu-id="367b2-138">在“创建事件中心”页面上，单击“**创建**”。</span><span class="sxs-lookup"><span data-stu-id="367b2-138">On the Event Hubs creation page, click **Create**.</span></span>
1. <span data-ttu-id="367b2-139">填写事件中心命名空间创建详细信息，然后单击“**创建**”。</span><span class="sxs-lookup"><span data-stu-id="367b2-139">Fill in the Event Hubs namespace creation details, and then click **Create**.</span></span>  
1. <span data-ttu-id="367b2-140">预配事件中心命名空间后，转到该命名空间的页面。</span><span class="sxs-lookup"><span data-stu-id="367b2-140">When the Event Hub namespace is provisioned, go to the page for the namespace.</span></span>  
1. <span data-ttu-id="367b2-141">单击“**事件中心**”和“**+ 事件中心**”。</span><span class="sxs-lookup"><span data-stu-id="367b2-141">Click **Event Hubs** and **+ Event Hub**.</span></span>  
1. <span data-ttu-id="367b2-142">为新事件中心命名，然后单击“**创建**”。</span><span class="sxs-lookup"><span data-stu-id="367b2-142">Give a name to the new Event Hub, and click **Create**.</span></span>  
1. <span data-ttu-id="367b2-143">创建事件中心后，单击事件中心的名称，然后单击“**共享访问策略**”和“**+ 添加**”以添加新策略。</span><span class="sxs-lookup"><span data-stu-id="367b2-143">After the Event Hub has been created, click the name of the Event Hub, and then click **Shared access policies** and **+ Add** to add a new policy.</span></span>  
1. <span data-ttu-id="367b2-144">为策略命名，选中“**发送**”，然后单击“**创建**”。</span><span class="sxs-lookup"><span data-stu-id="367b2-144">Give a name to the policy, check **Send**, and click **Create**.</span></span>  
1. <span data-ttu-id="367b2-145">创建策略后，单击策略的名称以打开“详细信息”面板，然后复制“**连接字符串-主键**” 值。</span><span class="sxs-lookup"><span data-stu-id="367b2-145">After the policy has been created, click the name of the policy to open the details panel, and then copy the **Connection string-primary key** value.</span></span> <span data-ttu-id="367b2-146">记下该值，在下一步中你需要使用它。</span><span class="sxs-lookup"><span data-stu-id="367b2-146">Write it down; you'll need it for the next step.</span></span>  

##### <a name="configuring-the-azure-key-vault"></a><span data-ttu-id="367b2-147">配置 Azure 密钥保管库</span><span class="sxs-lookup"><span data-stu-id="367b2-147">Configuring the Azure Key Vault</span></span>

<span data-ttu-id="367b2-148">为了安全地访问事件中心并允许密钥轮换，Microsoft Graph 将通过 Azure 密钥保管库获取事件中心的连接字符串。</span><span class="sxs-lookup"><span data-stu-id="367b2-148">In order to access the Event Hub securely and to allow for key rotations, Microsoft Graph gets the connection string to the Event Hub through Azure Key Vault.</span></span>  
<span data-ttu-id="367b2-149">在本节中，你将：</span><span class="sxs-lookup"><span data-stu-id="367b2-149">In this section, you will:</span></span>

- <span data-ttu-id="367b2-150">创建 Azure 密钥保管库以存储密钥。</span><span class="sxs-lookup"><span data-stu-id="367b2-150">Create an Azure Key Vault to store secret.</span></span>
- <span data-ttu-id="367b2-151">将连接字符串作为密钥添加到事件中心。</span><span class="sxs-lookup"><span data-stu-id="367b2-151">Add the connection string to the Event Hub as a secret.</span></span>
- <span data-ttu-id="367b2-152">为 Microsoft Graph 添加访问策略以访问密钥。</span><span class="sxs-lookup"><span data-stu-id="367b2-152">Add an access policy for Microsoft Graph to access the secret.</span></span>

<span data-ttu-id="367b2-153">步骤：</span><span class="sxs-lookup"><span data-stu-id="367b2-153">Steps:</span></span>

1. <span data-ttu-id="367b2-154">打开浏览器以访问 [Azure 门户](https://portal.azure.com)。</span><span class="sxs-lookup"><span data-stu-id="367b2-154">Open a browser to the [Azure Portal](https://portal.azure.com).</span></span>
1. <span data-ttu-id="367b2-155">选择“**创建资源**”。</span><span class="sxs-lookup"><span data-stu-id="367b2-155">Select **Create a resource**.</span></span>
1. <span data-ttu-id="367b2-156">在搜索栏中键入“**密钥保管库**”。</span><span class="sxs-lookup"><span data-stu-id="367b2-156">Type **Key Vault** in the search bar.</span></span>
1. <span data-ttu-id="367b2-157">选择“**密钥保管库**”建议。</span><span class="sxs-lookup"><span data-stu-id="367b2-157">Select the **Key Vault** suggestion.</span></span> <span data-ttu-id="367b2-158">此时将加载“创建密钥保管库”页面。</span><span class="sxs-lookup"><span data-stu-id="367b2-158">The Key Vault creation page will load.</span></span>
1. <span data-ttu-id="367b2-159">在“创建密钥保管库”页面上，单击“**创建**”。</span><span class="sxs-lookup"><span data-stu-id="367b2-159">On the Key Vault creation page, click **Create**.</span></span>  
1. <span data-ttu-id="367b2-160">填写密钥保管库创建详细信息，然后单击“**审阅 + 创建**”和“**创建**”。</span><span class="sxs-lookup"><span data-stu-id="367b2-160">Fill in the Key Vault creation details, and then click **Review + Create** and **Create**.</span></span>  
1. <span data-ttu-id="367b2-161">使用通知中的“**转到资源**”转到新创建的密钥保管库。</span><span class="sxs-lookup"><span data-stu-id="367b2-161">Go to the newly crated key vault using the **Go to resource** from the notification.</span></span>  
1. <span data-ttu-id="367b2-162">复制 **DNS 名称**；在下一步中你需要使用它。</span><span class="sxs-lookup"><span data-stu-id="367b2-162">Copy the **DNS name**; you will need it for the next step.</span></span>  
1. <span data-ttu-id="367b2-163">转到“**密钥**”，然后单击“**+ 生成/导入**”。</span><span class="sxs-lookup"><span data-stu-id="367b2-163">Go to **Secrets** and click **+ Generate/Import**.</span></span>  
1. <span data-ttu-id="367b2-164">为密钥命名，并保留名称供以后使用，在下一步中你需要使用它。</span><span class="sxs-lookup"><span data-stu-id="367b2-164">Give a name to the secret, and keep the name for later; you will need it for the next step.</span></span> <span data-ttu-id="367b2-165">对于该值，请粘贴在“事件中心”步骤中生成的连接字符串。</span><span class="sxs-lookup"><span data-stu-id="367b2-165">For the value, paste in the connection string you generated at the Event Hubs step.</span></span> <span data-ttu-id="367b2-166">单击“**创建**”。</span><span class="sxs-lookup"><span data-stu-id="367b2-166">Click **Create**.</span></span>  
1. <span data-ttu-id="367b2-167">单击“**访问策略**”和“**+ 添加访问策略**”。</span><span class="sxs-lookup"><span data-stu-id="367b2-167">Click **Access Policies** and **+ Add Access Policy**.</span></span>  
1. <span data-ttu-id="367b2-168">对于“**密钥权限**”，选择“**获取**”；对于“**选择主体**”，选择“**Microsoft Graph 更改跟踪**”。</span><span class="sxs-lookup"><span data-stu-id="367b2-168">For **Secret permissions**, select **Get**, and for **Select Principal**, select **Microsoft Graph Change Tracking**.</span></span> <span data-ttu-id="367b2-169">单击“**添加**”。</span><span class="sxs-lookup"><span data-stu-id="367b2-169">Click **Add**.</span></span>  

### <a name="creating-the-subscription-and-receiving-notifications"></a><span data-ttu-id="367b2-170">创建订阅并接收通知</span><span class="sxs-lookup"><span data-stu-id="367b2-170">Creating the subscription and receiving notifications</span></span>

<span data-ttu-id="367b2-171">创建所需的 Azure 密钥保管库和 Azure 事件中心服务后，你将能够创建订阅并开始通过 Azure 事件中心接收更改通知。</span><span class="sxs-lookup"><span data-stu-id="367b2-171">After you create the required Azure KeyVault and Azure Event Hubs services, you will be able to create your subscription and start receiving change notifications via Azure Event Hubs.</span></span>

#### <a name="creating-the-subcription"></a><span data-ttu-id="367b2-172">创建订阅</span><span class="sxs-lookup"><span data-stu-id="367b2-172">Creating the subcription</span></span>

<span data-ttu-id="367b2-173">使用事件中心订阅更改通知与使用 Webhook 订阅更改通知几乎相同。</span><span class="sxs-lookup"><span data-stu-id="367b2-173">Subscriptions to change notifications with Event Hubs are almost identical to change notifications with webhooks.</span></span> <span data-ttu-id="367b2-174">主要区别在于前者依赖事件中心来传送通知。</span><span class="sxs-lookup"><span data-stu-id="367b2-174">The key difference is that they rely on Event Hubs to deliver notifications.</span></span> <span data-ttu-id="367b2-175">所有其他操作都类似，包括[创建订阅](/graph/api/subscription-post-subscriptions?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="367b2-175">All other operations are similar, including [subscription creation](/graph/api/subscription-post-subscriptions?view=graph-rest-beta).</span></span>  

<span data-ttu-id="367b2-176">创建订阅期间的主要区别是 **notificationUrl**。</span><span class="sxs-lookup"><span data-stu-id="367b2-176">The main difference during subscription creation will be the **notificationUrl**.</span></span> <span data-ttu-id="367b2-177">必须将其设置为 `EventHub:https://<azurekeyvaultname>.vault.azure.net/secrets/<secretname>?tenantId=<domainname>`，并使用以下值：</span><span class="sxs-lookup"><span data-stu-id="367b2-177">You must set it to `EventHub:https://<azurekeyvaultname>.vault.azure.net/secrets/<secretname>?tenantId=<domainname>`, with the following values:</span></span>

- <span data-ttu-id="367b2-178">`azurekeyvaultname` - 创建密钥保管库时为其提供的名称。</span><span class="sxs-lookup"><span data-stu-id="367b2-178">`azurekeyvaultname` - The name you gave to the key vault when you created it.</span></span> <span data-ttu-id="367b2-179">可在 DNS 名称中找到它。</span><span class="sxs-lookup"><span data-stu-id="367b2-179">Can be found in the DNS name.</span></span>
- <span data-ttu-id="367b2-180">`secretname` - 创建密钥时为其提供的名称。</span><span class="sxs-lookup"><span data-stu-id="367b2-180">`secretname` - The name you gave to the secret when you created it.</span></span> <span data-ttu-id="367b2-181">可在 Azure 密钥保管库的“**密钥**”页面上找到它。</span><span class="sxs-lookup"><span data-stu-id="367b2-181">Can be found on the Azure Key Vault **Secrets** page.</span></span>
- <span data-ttu-id="367b2-182">`domainname` - 租户的名称；例如，consto.onmicrosoft.com 或 contoso.com。</span><span class="sxs-lookup"><span data-stu-id="367b2-182">`domainname` - The name of your tenant; for example, consto.onmicrosoft.com or contoso.com.</span></span> <span data-ttu-id="367b2-183">由于此域将用于访问 Azure 密钥保管库，因此请务必使其与包含 Azure 密钥保管库的 Azure 订阅所使用的域相匹配。</span><span class="sxs-lookup"><span data-stu-id="367b2-183">Because this domain will be used to access the Azure Key Vault, it is important that it matches the domain used by the Azure subscription that holds the Azure Key Vault.</span></span> <span data-ttu-id="367b2-184">若要获取此信息，可转到你创建的 Azure 密钥保管库的概述页面，并单击该订阅。</span><span class="sxs-lookup"><span data-stu-id="367b2-184">To get this information, you can go to the overview page of the Azure Key Vault you created and click the subscription.</span></span> <span data-ttu-id="367b2-185">域名将显示在“**目录**”字段下。</span><span class="sxs-lookup"><span data-stu-id="367b2-185">The domain name is displayed under the **Directory** field.</span></span>

#### <a name="receiving-notifications"></a><span data-ttu-id="367b2-186">接收通知</span><span class="sxs-lookup"><span data-stu-id="367b2-186">Receiving notifications</span></span>

<span data-ttu-id="367b2-187">事件现在将通过事件中心传送到你的应用程序中。</span><span class="sxs-lookup"><span data-stu-id="367b2-187">Events will be now delivered to your application by Event Hubs.</span></span> <span data-ttu-id="367b2-188">有关详细信息，请参阅事件中心文档中的[接收事件](/azure/event-hubs/get-started-dotnet-standard-send-v2#receive-events)。</span><span class="sxs-lookup"><span data-stu-id="367b2-188">For details, see [receiving events](/azure/event-hubs/get-started-dotnet-standard-send-v2#receive-events) in the Event Hubs documentation.</span></span>

<span data-ttu-id="367b2-189">在应用程序中接收通知之前，你需要创建另一个具有“侦听”权限的共享访问策略并获取连接字符串，类似于[配置 Azure 事件中心](#configuring-the-azure-event-hub)中列出的步骤。</span><span class="sxs-lookup"><span data-stu-id="367b2-189">Before you can receive the notifications in your application, you'll need to create another shared access policy with a "Listen" permission and obtain the connection string, similar to the steps listed in [Configuring the Azure Event Hub](#configuring-the-azure-event-hub).</span></span>

> <span data-ttu-id="367b2-190">**注意：** 为应用程序创建单独的策略来侦听事件中心消息，而不是重用在 Azure 密钥保管库中设置的相同连接字符串。</span><span class="sxs-lookup"><span data-stu-id="367b2-190">**Note:** Create a separate policy for the application that listens to Event Hubs messages instead of reusing the same connection string you set in Azure KeyVault.</span></span> <span data-ttu-id="367b2-191">这可确保解决方案的每个组件仅具有所需的权限，并遵循最低权限安全原则。</span><span class="sxs-lookup"><span data-stu-id="367b2-191">This ensures that each component of the solution has only the permissions it needs and follows the least permissions security principle.</span></span>

> <span data-ttu-id="367b2-192">**注意：** 应用程序会在每次创建新订阅时收到验证消息。</span><span class="sxs-lookup"><span data-stu-id="367b2-192">**Note:** Your application receives validation messages whenever it creates a new subscription.</span></span> <span data-ttu-id="367b2-193">应忽略这些通知。</span><span class="sxs-lookup"><span data-stu-id="367b2-193">You should ignore these notifications.</span></span> <span data-ttu-id="367b2-194">下面的示例表示验证消息的正文。</span><span class="sxs-lookup"><span data-stu-id="367b2-194">The following example represents the body of a validation message.</span></span>

```json
 {
    "value":[
        {
            "subscriptionId":"NA",
            "subscriptionExpirationDateTime":"NA",
            "clientState":"NA",
            "changeType":"Validation: Testing client application reachability for subscription Request-Id: 522a8e7e-096a-494c-aaf1-ac0dcfca45b7",
            "resource":"NA",
            "resourceData":{
                "@odata.type":"NA",
                "@odata.id":"NA",
                "id":"NA"
            }
        }
    ]
}
```

### <a name="what-happens-if-the-microsoft-graph-change-tracking-application-is-missing"></a><span data-ttu-id="367b2-195">如果缺少 Microsoft Graph 更改跟踪应用程序会怎样？</span><span class="sxs-lookup"><span data-stu-id="367b2-195">What happens if the Microsoft Graph change tracking application is missing?</span></span>

<span data-ttu-id="367b2-196">租户中可能缺少 **Microsoft Graph 更改跟踪** 服务主体，这取决于租户的创建时间和管理操作。</span><span class="sxs-lookup"><span data-stu-id="367b2-196">It's possible that the **Microsoft Graph Change Tracking** service principal is missing from your tenant, depending on when the tenant was created and administrative operations.</span></span> <span data-ttu-id="367b2-197">若要解决此问题，请在 [Microsoft Graph 浏览器](https://developer.microsoft.com/zh-CN/graph/graph-explorer)中运行[以下查询](https://developer.microsoft.com/zh-CN/graph/graph-explorer?request=servicePrincipals&method=POST&version=v1.0&GraphUrl=https://graph.microsoft.com&requestBody=eyJhcHBJZCI6IjBiZjMwZjNiLTRhNTItNDhkZi05YTgyLTIzNDkxMGM0YTA4NiJ9)。</span><span class="sxs-lookup"><span data-stu-id="367b2-197">To resolve this issue, run [the following query](https://developer.microsoft.com/zh-CN/graph/graph-explorer?request=servicePrincipals&method=POST&version=v1.0&GraphUrl=https://graph.microsoft.com&requestBody=eyJhcHBJZCI6IjBiZjMwZjNiLTRhNTItNDhkZi05YTgyLTIzNDkxMGM0YTA4NiJ9) in [Microsoft Graph Explorer](https://developer.microsoft.com/zh-CN/graph/graph-explorer).</span></span>

<span data-ttu-id="367b2-198">查询详细信息：</span><span class="sxs-lookup"><span data-stu-id="367b2-198">Query details:</span></span>

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals
{
    "appId": "0bf30f3b-4a52-48df-9a82-234910c4a086"
}
```

> <span data-ttu-id="367b2-199">**注意：** 运行此查询会导致访问被拒绝。</span><span class="sxs-lookup"><span data-stu-id="367b2-199">**Note:** You can get an access denied running this query.</span></span> <span data-ttu-id="367b2-200">在这种情况下，请选择左上角帐户名称旁边的齿轮图标。</span><span class="sxs-lookup"><span data-stu-id="367b2-200">In this case, select the gear icon next to your account name in the top left corner.</span></span> <span data-ttu-id="367b2-201">然后选择“**选择权限**”并搜索 **Application.ReadWrite.All**。</span><span class="sxs-lookup"><span data-stu-id="367b2-201">Then select **Select Permissions** and search for **Application.ReadWrite.All**.</span></span> <span data-ttu-id="367b2-202">检查权限，然后选择“**同意**”。</span><span class="sxs-lookup"><span data-stu-id="367b2-202">Check the permission and select **Consent**.</span></span> <span data-ttu-id="367b2-203">同意此新权限后，再次运行请求。</span><span class="sxs-lookup"><span data-stu-id="367b2-203">After consenting to this new permission, run the request again.</span></span>

> <span data-ttu-id="367b2-204">**注意：** 此 API 仅适用于学校或工作帐户，而不适用于个人帐户。</span><span class="sxs-lookup"><span data-stu-id="367b2-204">**Note:** This API only works with a school or work account, not with a personal account.</span></span> <span data-ttu-id="367b2-205">请确保使用域中的帐户登录。</span><span class="sxs-lookup"><span data-stu-id="367b2-205">Make sure that you are signed in with an account on your domain.</span></span>

<span data-ttu-id="367b2-206">或者，你也可以使用此 [Azure Active Directory PowerShell](/powershell/azure/active-directory/install-adv2?view=azureadps-2.0) 脚本添加缺少的服务主体。</span><span class="sxs-lookup"><span data-stu-id="367b2-206">Alternatively, you can use this [Azure Active Directory PowerShell](/powershell/azure/active-directory/install-adv2?view=azureadps-2.0) script to add the missing service principal.</span></span>

```PowerShell
Connect-AzureAD -TenantId <tenant-id>
# replace tenant-id by the id of your tenant.
New-AzureADServicePrincipal -AppId 0bf30f3b-4a52-48df-9a82-234910c4a086
```

## <a name="next-steps"></a><span data-ttu-id="367b2-207">后续步骤</span><span class="sxs-lookup"><span data-stu-id="367b2-207">Next steps</span></span>

<span data-ttu-id="367b2-208">请参阅下面的 Azure 事件中心快速入门：</span><span class="sxs-lookup"><span data-stu-id="367b2-208">See the following Azure Event Hubs quick starts:</span></span>

- [<span data-ttu-id="367b2-209">.NET Core</span><span class="sxs-lookup"><span data-stu-id="367b2-209">.NET Core</span></span>](/azure/event-hubs/get-started-dotnet-standard-send-v2)
- [<span data-ttu-id="367b2-210">Java</span><span class="sxs-lookup"><span data-stu-id="367b2-210">Java</span></span>](/azure/event-hubs/event-hubs-java-get-started-send)
- [<span data-ttu-id="367b2-211">Python</span><span class="sxs-lookup"><span data-stu-id="367b2-211">Python</span></span>](/azure/event-hubs/get-started-python-send-v2)
- [<span data-ttu-id="367b2-212">JavaScript</span><span class="sxs-lookup"><span data-stu-id="367b2-212">JavaScript</span></span>](/azure/event-hubs/get-started-node-send-v2)
