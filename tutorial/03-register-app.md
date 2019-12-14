---
ms.openlocfilehash: 4e62f08217ab00427218cd1815d66d80fd2802de
ms.sourcegitcommit: 2af94da662c454e765b32edeb9406812e3732406
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/13/2019
ms.locfileid: "40018823"
---
<!-- markdownlint-disable MD002 MD041 -->

<span data-ttu-id="8c601-101">In dieser Übung erstellen Sie mithilfe des Azure Active Directory Admin Center eine neue Azure AD Anwendung.</span><span class="sxs-lookup"><span data-stu-id="8c601-101">In this exercise you will create a new Azure AD application using the Azure Active Directory admin center.</span></span>

1. <span data-ttu-id="8c601-102">Öffnen Sie einen Browser, und navigieren Sie zum [Azure Active Directory Admin Center](https://aad.portal.azure.com). Melden Sie sich mit einem **persönlichen Konto** (auch: Microsoft-Konto) oder einem **Geschäfts- oder Schulkonto** an.</span><span class="sxs-lookup"><span data-stu-id="8c601-102">Open a browser and navigate to the [Azure Active Directory admin center](https://aad.portal.azure.com) and login using a **personal account** (aka: Microsoft Account) or **Work or School Account**.</span></span>

1. <span data-ttu-id="8c601-103">Wählen Sie in der linken Navigationsleiste **Azure Active Directory** aus, und wählen Sie dann **App-Registrierungen** unter **Verwalten** aus.</span><span class="sxs-lookup"><span data-stu-id="8c601-103">Select **Azure Active Directory** in the left-hand navigation, then select **App registrations** under **Manage**.</span></span>

    ![<span data-ttu-id="8c601-104">Ein Screenshot der APP-Registrierungen</span><span class="sxs-lookup"><span data-stu-id="8c601-104">A screenshot of the App registrations</span></span> ](./images/aad-portal-app-registrations.png)

1. <span data-ttu-id="8c601-105">Wählen Sie **Neue Registrierung** aus.</span><span class="sxs-lookup"><span data-stu-id="8c601-105">Select **New registration**.</span></span> <span data-ttu-id="8c601-106">Legen Sie auf der Seite **Anwendung registrieren** die Werte wie folgt fest.</span><span class="sxs-lookup"><span data-stu-id="8c601-106">On the **Register an application** page, set the values as follows.</span></span>

    - <span data-ttu-id="8c601-107">Legen Sie **Name** auf `Java Graph Tutorial` fest.</span><span class="sxs-lookup"><span data-stu-id="8c601-107">Set **Name** to `Java Graph Tutorial`.</span></span>
    - <span data-ttu-id="8c601-108">Legen Sie **Unterstützte Kontotypen** auf **Konten in allen Organisationsverzeichnissen und persönliche Microsoft-Konten** fest.</span><span class="sxs-lookup"><span data-stu-id="8c601-108">Set **Supported account types** to **Accounts in any organizational directory and personal Microsoft accounts**.</span></span>
    - <span data-ttu-id="8c601-109">Lassen Sie **URI umleiten** leer.</span><span class="sxs-lookup"><span data-stu-id="8c601-109">Leave **Redirect URI** empty.</span></span>

    ![Screenshot der Seite "Anwendung registrieren"](./images/aad-register-an-app.png)

1. <span data-ttu-id="8c601-111">Wählen Sie **Registrieren** aus.</span><span class="sxs-lookup"><span data-stu-id="8c601-111">Choose **Register**.</span></span> <span data-ttu-id="8c601-112">Kopieren Sie auf der Seite **Java Graph Tutorial** den Wert der **Anwendungs-ID (Client)** , und speichern Sie ihn, die Sie im nächsten Schritt benötigen.</span><span class="sxs-lookup"><span data-stu-id="8c601-112">On the **Java Graph Tutorial** page, copy the value of the **Application (client) ID** and save it, you will need it in the next step.</span></span>

    ![Ein Screenshot der Anwendungs-ID der neuen App-Registrierung](./images/aad-application-id.png)

1. <span data-ttu-id="8c601-114">Klicken Sie auf den Link **Umleitungs-URI hinzufügen** .</span><span class="sxs-lookup"><span data-stu-id="8c601-114">Select the **Add a Redirect URI** link.</span></span> <span data-ttu-id="8c601-115">Suchen Sie auf der Seite " **Umleitungs-URIs** " den Abschnitt **vorgeschlagene Umleitungs-URIs für öffentliche Clients (Mobile, Desktop)** .</span><span class="sxs-lookup"><span data-stu-id="8c601-115">On the **Redirect URIs** page, locate the **Suggested Redirect URIs for public clients (mobile, desktop)** section.</span></span> <span data-ttu-id="8c601-116">Wählen Sie `https://login.microsoftonline.com/common/oauth2/nativeclient` den URI aus.</span><span class="sxs-lookup"><span data-stu-id="8c601-116">Select the `https://login.microsoftonline.com/common/oauth2/nativeclient` URI.</span></span>

    ![Screenshot der Seite "Umleitungs-URIs"](./images/aad-redirect-uris.png)

1. <span data-ttu-id="8c601-118">Suchen Sie den **standardmäßigen Clienttyp** Abschnitt, und ändern Sie die Option **Anwendung als öffentlichen Client** Umschalten auf **Ja**, und wählen Sie dann **Speichern**aus.</span><span class="sxs-lookup"><span data-stu-id="8c601-118">Locate the **Default client type** section and change the **Treat application as a public client** toggle to **Yes**, then choose **Save**.</span></span>

    ![Ein Screenshot des Typs "Standard Clienttyp"](./images/aad-default-client-type.png)
